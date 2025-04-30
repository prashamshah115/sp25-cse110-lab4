1) Line 12 prints 3 to the console. This is because var has function-scope and not block-scope, and so i is still defined at line 12, and since its value is 3, 3 is printed out to console. 

2) Line 13 here will print out 150 to the console. Once again, since discountedPrice is declared with var which has function scope and not block scope, discountedPrice carries the value 150 into line 13. 

3) Line 14 prints 150. finalPrice is function scoped and inside the for loop, its last assignment is 150, which persists in function scope. 

4) This function returns : [50,100,150]. This is because discounted is an array with function scope, and essentially the for loop takes every value in price and halves it. 

5) Here, line 12 will return a ReferenceError. This is becuase i is declared with the let keyword which only has block scope and so, outside the for loop, ie in line 12, it is not defined. 

6) Once again, in line 13, we get a ReferenceError. discountedPrice is defined with the let keyword inside the for loop, and is not defined outside of it. 

7) At line 14, we get the value 150. finalPrice is defined before for loop, and so has function scope and is defined with value 150, at line 14. 

8) This function returns : [50,100,150]. This is because discounted is an array with function scope, and essentially the for loop takes every value in price and halves it. 

9) Line 11 returns an error. We get a ReferenceError as i is defined with let, and only has block scope. 

10) Line 12 prints the value 3 to the console. This is because length is declared with const before for loop and is defined at line 12, and no attempts have been made to change its value. 

11) const prevents reassignment and not mutation. We can pushto discounted, and so the function will return [50,100,150]. 

12) A. student.name
    B. student['Grad Year']
    C. student.greeting()
    D. student['Favorite Teacher'].name
    E. student.courseload[0]

13) A. '32'. This is because since '3' is a string, + acts as the string concatenation operator. 
    B. 1 as - is not defined for strings and JS tries to convert both to numbers.
    C. 3 as null is coerced to 0 in arithmetic operations. 
    D. '3null' as + with a string means coercion to string happens
    E. 4 as true is coerced to 1. 
    F. 0 as false is 0 and null is 0 so 0+0=0
    G. '3undefined' as + with a string means coercion to string. 
    H. NaN. - tries to coerce both to numbers and so undefined becomed NaN. 

14) A. true as JS will convert '2' to 2 
    B. we use lexicographic comparison and since '2' comes after '1' we get false. 
    C. true as == does type coercion. 
    D. false as === checks value and type. 
    E. false as true is coerced to 1. 
    F. true as Boolean(2) is true. 

15) == is loose equality and it does type coercion and does not check for type. Eg. 2 == '2' will return true. === is a strict equality and does not do type coercion while checking type. 2 === '2' will return false. 

17) The result of this function call is [2,4,6]. modifyArray([1,2,3], doSomething) is called. Then, inside modifyArray, a new array newArr = [] is created. The function loops through input array, and for each iteration calls callback ie doSomething so for callback(1) -> returns 2, and 4 and 6 respectively for callback(2) and callback(3). Each return value is pushed to newArr. 

19) 1
    4
    3
    2

