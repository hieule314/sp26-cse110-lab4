1. Line 12 prints:
3

Explanation: i is declared with var inside the for loop. Because var is function-scoped, i is accessible after the loop ends. The loop stops when i becomes 3.

2. Line 13 prints:
150

Explaination: discountedPrice is declared with var inside the for loop, so it is function-scoped. After the loop finishes, it keeps the last value, which is 300 * (1 - 0.5) = 150

3. Line 14 prints:
150

Explaination: finalPrice is declared with var outside the loop and updated each loop iteration. After the final iteration, the value is 150.

4. The function returns:
[50, 100, 150]

Explaination: each price is multiplied by (1 - discount), so the price becomes 50, 100, and 150. These values are pushed into the discounted array.

5. Line 12 causes an error:
ReferenceError: i is not defined

Explaination: i is declared with let inside the for loop, so it is block-scoped and cannot be accessed outside the loop.

6. Line 13 causes an error:
ReferenceError: discountedPrice is not defined

Explaination: discountedPrice is declared with let inside the for loop, so it only exists inside the loop block.

7. Line 14 prints:
150

Explaination: finalPrice is declared with let outside the for loop, so it is accessible after the loop. It stores the last calculated final price; 150.

8. The function returns:
[50, 100, 150]

Explaination: discounted is declared with let outside the loop and it is still accessible at the return. Each calculated finalPrice is pushed into the discounted array.

9. Line 11 causes an error:
ReferenceError: i is not defined

Explaination: i is declared with let inside the for loop, so it is block-scoped and cannot be accessed outside the loop.

10. Line 12 prints:
3

Explaination: length is declared with const inside the function but outside the loop, so it is accessible on line 12. Length is 3 since prices has 3 elements.

11. The function returns:
[50, 100, 150]

Explaination: discounted is declared with const, but the array itself can still be modified. This code does not reassign discounted; it only pushes values into the array.

