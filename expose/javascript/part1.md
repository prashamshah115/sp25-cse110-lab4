1) Line 9 prints : "values added: 20"
This is because add === true and so, the if block runs, and result is assigned 10 + 10 = 20 and so, it is logged. 

2) Line 13 prints : "final result: 20". Since result was used with var, it is function-scoped and so, it is available throughout entire function and not just the if. If we used let or const, we would've gotten a ReferenceError. 

3) var is dangerous and outdated and so we should not use it. It is function-scoped and not block-scoped, you could hoist with var, and could accidentally redeclare, all not desirable. Unless maintaining old code, we probably should not use var. 
   
4) Here, line 9 prints : "values added: 20". The if condition is true, and let result line declares result inside the block scope, and result is updated to 20. 

5) Line 13 now will give a ReferenceError as result is not defined here. let is block-scoped, which means result will only exist in the { } part of if. Line 13 is outside that block, and so result is not accessible there and JavaScript is not able to find that variable. 

6) Line 9 will throw a TypeError as we are attempting assignment to a constant variable. This is because once we assign a value to a constant, attempts to reassign are illegal. 

7) Line 13 will never be reached because execution fails at line 6 due to the TypeError. Even if we did reach here, it would throw a ReferenceError as result is not defined in that scope. 