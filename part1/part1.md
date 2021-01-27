1. At line 11, the length of prices will be printed to the console. This happens because var i will remain after the for loop is over since var i is a function variable.
2. At line 12, the last assignment to `discountedPrice` will remain after the for loop is over since var discountedPrice is a function variable. Thus, the last assignment to discountedPrice will be printed to the console.
3. At line 13, the last assignment to `finalPrice` will be printed. This happens because var finalPrice will remain after the for loop is over since `var finalPrice` is a function variable.
4. discountPrices([100, 200, 300], .5) will return the discounted array which would be `[50, 100, 150]`. The function discountPrices iterates through [100, 200, 300] array, so that each element in this array will get its discountedPrice by multiplying the price at var i in array prices by (1 - 0.5). Then the finalPrice is found by rounding the (discountedPrice * 100)/100. The finalPrice will at the end of each iteration will then be pushed to the discounted array, which will then be the output of this function.
5. Line 11 won't output anything and will cause an error since the value of i is out of scope. It is out of scope because i is only visible inside of the for loop.
6. Line 12 won't output anything and will cause an error since the value of discountedPrice is out of scope. It is out of scope because discountedPrice is only visible inside of the for loop.
7. Line 13  will print the last assigned value for finalPrice. This line actually works because the value for finalPrice is assigned where it's referenced and within the scope of the function.
8. discountPrices([100, 200, 300], .5) will return the discounted array which would be `[50, 100, 150]`, only if the errors from line 11 and 12 don't get in the way. The function will iterate over the elements in prices and will find the discountedPrice and finalPrice for each element and push that into the array. This array discounted will then be returned.
9. Line 11 won't output anything and will cause an error since the value of i is out of scope. It is out of scope because i is only visible inside of the for loop. Since the console.log command is also out of scope of the for loop, there will be issues.
10. Line 12 won't output anything and will cause an error since it's type is const which doesn't allow the value to be reassigned. Since the console.log command is also out of scope of the for loop, there will be issues.
11. Line 13 will print the value of finalPrice which should be `0`. This works since there are no scope problems and since the console.log command is called within the function scope.
12. discountPrices([100, 200, 300], .5) will return the discounted array `[0, 0, 0]`. This is because the scoping errors and const errors will prohibit the function from being able to compute the discountedPrice and finalPrice.
13.  
    A. `student["name"];`  
    B. `student["Grad Year"];`  
    C. `student.greeting();`  
    D. `student["Favorite Teacher"]["name"]`  
    E. `student["courseLoad"][0]`  
14. Arithmetic  
    A. '3' + 2  
    This appends 2 to the '3' string, which will output `'32'`.  
    B. '3' - 2  
    This will convert the strings to numbers and will subtract 3-2, which will output `1`.  
    C. 3 + null  
    The null will be considered a 0, so it will calculate 3 + 0, which will output `3`.  
    D. '3' + null  
    This appends null to the '3' string, so the output will be 3null.  
    E. true + 3  
    The true will be considered a 1, so it will calculate 1 + 3, which will output `4`.  
    F. false + null  
    The false and the null will be considered 0's, so it will calculate 0 + 0, which will output `0`.  
    G. "3" + undefined  
    This appends undefined to the "3" string, which will output `3undefined`.  
    H. "3" - undefined  
    This is not good arithmetic, so the output will be `NaN`.
15. Comparison  
    A. '2' > 1  
    This will convert the '2' string into a number and will compare the integers. Since 2 is greater than 1, the output will be `true`.  
    B. '2' < '12'  
    This will compare the strings and the output will be `false`.  
    C. 2 == '2'  
    This will convert the '2' string into a number and will check to see if the integers are equal. The output will be `true`.  
    D. 2 === '2'  
    This will attempt to check if the 2 integer and the '2' string are equal. The output will be `false`.  
    E. true == 2  
    This will check to see if the true is equal to 2. Since the true is considered 1, the output will be `false`.  
    F. true === Boolean(2)  
    This will check to see if true is equal to Boolean(2). Since Boolean(2) returns true, the output will be `true`.  
16. == vs. ===  
The == makes sure that the two being compared are the same type by converting it, but the === does not do conversions when checking for equality.  
17. Since Boolean(2) returns true, and true == true is true, the output from this code snippet will be Hello!.  
18. part1/part1-question18.js  
19. An array `[6, 8, 10]` will be returned. The function modifyArray iterates through the given array [1, 2, 3] and for each index the function runs the callback method `doSomething`, which will return the value `(value + 2) * 2`. `doSomething` will run the callback on the value `value + 2` which will then be doubled. Then the value will be added to the array `newArr`, which will then be returned.
20. part1/part1-question20.jsv
21. Output:  
```
1  
4  
2  
3  
```
    
