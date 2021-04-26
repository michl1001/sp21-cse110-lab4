# 1A

1. values added:  20
2. values added:  20
3. values added:  20
4. C:\Users\Michl1001\Documents\College\CSE 110\LAB4\sp21-cse110-lab4\part1\part1a.js:8
    console.log('values added: ', result);
                                  ^

ReferenceError: result is not defined
    at sumValues (C:\Users\Michl1001\Documents\College\CSE 110\LAB4\sp21-cse110-lab4\part1\part1a.js:8:35)
    at Object.<anonymous> (C:\Users\Michl1001\Documents\College\CSE 110\LAB4\sp21-cse110-lab4\part1\part1a.js:12:1)
    at Module._compile (internal/modules/cjs/loader.js:956:30)
    at Object.Module._extensions..js (internal/modules/cjs/loader.js:973:10)
    at Module.load (internal/modules/cjs/loader.js:812:32)
    at Function.Module._load (internal/modules/cjs/loader.js:724:14)
    at Function.Module.runMain (internal/modules/cjs/loader.js:1025:10)
    at internal/main/run_main_module.js:17:11

In this case, "let" only declares a variable in a certian scope where the let statement is. Thus, this line tries to access the variable in a location outside of that scope (the if staement in this case) and thus the variable access throws an error.

5. C:\Users\Michl1001\Documents\College\CSE 110\LAB4\sp21-cse110-lab4\part1\part1a.js:4
        result = num1 + num2;
               ^

TypeError: Assignment to constant variable.
    at sumValues (C:\Users\Michl1001\Documents\College\CSE 110\LAB4\sp21-cse110-lab4\part1\part1a.js:4:16)
    at Object.<anonymous> (C:\Users\Michl1001\Documents\College\CSE 110\LAB4\sp21-cse110-lab4\part1\part1a.js:12:1)
    at Module._compile (internal/modules/cjs/loader.js:956:30)
    at Object.Module._extensions..js (internal/modules/cjs/loader.js:973:10)
    at Module.load (internal/modules/cjs/loader.js:812:32)
    at Function.Module._load (internal/modules/cjs/loader.js:724:14)
    at Function.Module.runMain (internal/modules/cjs/loader.js:1025:10)
    at internal/main/run_main_module.js:17:11

This error occurs before we hit this line. This error occurs because we try to edit a constant vaiable after inital assignment.

6. C:\Users\Michl1001\Documents\College\CSE 110\LAB4\sp21-cse110-lab4\part1\part1a.js:4
        result = num1 + num2;
               ^

TypeError: Assignment to constant variable.
    at sumValues (C:\Users\Michl1001\Documents\College\CSE 110\LAB4\sp21-cse110-lab4\part1\part1a.js:4:16)
    at Object.<anonymous> (C:\Users\Michl1001\Documents\College\CSE 110\LAB4\sp21-cse110-lab4\part1\part1a.js:12:1)
    at Module._compile (internal/modules/cjs/loader.js:956:30)
    at Object.Module._extensions..js (internal/modules/cjs/loader.js:973:10)
    at Module.load (internal/modules/cjs/loader.js:812:32)
    at Function.Module._load (internal/modules/cjs/loader.js:724:14)
    at Function.Module.runMain (internal/modules/cjs/loader.js:1025:10)
    at internal/main/run_main_module.js:17:11

This error occurs before we hit this line. This error occurs because we try to edit a constant vaiable after inital assignment.

# 1B

1. 3, This makes sense as this is the variable incremented in the loop and so when the loop ended, it was at that value of the length of the array prices which was 3 
2. 150, This makes sense as this variable was last set when the loop ended and that value was the last element of the prices array time (1 - .5) which is 300 * .5 which is 150 
3. 150, This makes sense as this variable was last set when the loop ended and that value was the last value of the variable from quesiton 2 multiplied and divided by 100 which is 150 
4. [50, 100, 150], this makes sense since this is the array of all the prices with discount giving price * .5. Thus, resulting array has values all half of the input array
5. Line 12 will cause an error as the variable i was declared with "let" which only declares the variable in local scope. As such, i only exists within the for loop that it was declared in so this line is accessing the variable outside it's scope.
6. Line 13 will cause an error as the variable discountedPrice was declared with "let" which only declares the variable in local scope. As such, discountedPrice only exists within the for loop that it was declared in so this line is accessing the variable outside it's scope.
7. Line 14 will print 150. This is because finalPrice was declared in the same scope as this line and this variable was last set when the loop ended and that value was the last value of discountPrice multiplied and divided by 100 which is 150
8.  [50, 100, 150], this makes sense since discount is declared in the same scope as  this is the array of all the prices with discount giving price * .5. Thus, the resulting discountPrice array has values all half of the input array
9.  Line 11 will cause an error as the variable i was declared with "let" which only declares the variable in local scope. As such, i only exists within the for loop that it was declared in so this line is accessing the variable outside it's scope.
10. Line 12 will print 3 as this was what length was set to during initializaion as constant and we are allow to access a constant value
11. [ 50, 100, 150 ], even though the array is declared as a constant, we are still allowed to push items to the array and so no error is given.
12. 
    A. student.name
    B. student['Grad Year']
    C. student.greeting()
    D. student['Favorite Teacher'].name
    E. student..courseload[0]
13. 
    A. "32" - this result is because one of the digits is encased by quotes and so the plus sign is interpreted as concatenation for strings
    B. 1 - this result is because there is no minus sign that works with strings so the digits are both interpreted as a numeric math substraction expression
    C. 3 - this is because null can be represented as a "0" value and so with 3 being a number, null is interpreted as a number with value 0 and so we get 3 + 0 = 3
    D. "3null" - since 3 was in quotes, it was interpreted as a character and so the plus sign was interpreted as concatenation and null as a string
    E. true represented by the number 1 to javacript and so with the numberic digit 3, the plus sign is interpreted as addition and true as 1
    F. Both numbers can be interpreted as the number 0, and with false next to the plus symbol, this expression is interpreted as addition with false and null being 0
    G. 3undefined - 3 is encased by quotes and so the plus sign is interpreted as concatenation for strings and so undefined is interpreted as a string
    H. NaN - There is no minus sign that works with strings so 3 is interpreted as a numeric with subtraction. However, taken as a number, undefined has no value and so the result of the math operation is invalid
14. 
    A. true - the comparison returns true as the 2 string is converted to a nummeric in the comparison and 2 is greater than 1
    B. false - the comparison make the 2 string into the 2 numeric but the 12 string only considers the fisrt digit when being made a numeric. Thus, the cmparison becomes 2 < 1 which is false
    C. true - this is true because the == sign doesn't consider type and so the 2 string is converted to the numeric 2
    D. false - this is false because the === check that the values have the same type which is not true
    E. false - this is false because true evaluates true as 1 and the string 2 as the numeric 2 which are not equal
    F. true - this is true as the boolean function takes any non-zero/non-null and defined value as true which is the same type and value as true.
15. == doesn't regard type, only value, when making the comparison whereas === requires that the values in the expression must have the same type
16. See file
17. [2, 4, 6] - The funciton modifyArray loops through the input array and uses each entry in array as the parameter input to the callback function. The results are each pushed to the returned newArr. For the given funciton doSomething, it returns double the input, so we can see that the full functions put together doubles each element of the inputed array and outputs an new array of those doubled elements.
18. See file
19. 
    1
    4
    3
    2
