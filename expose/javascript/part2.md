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

12.

a. student.name
b. student['Grad Year']
c. student.greeting()
d. student['Favorite Teacher'].name
e. student.courseLoad[0]

13. Arithmetic

A. '3' + '2' --> '32'

Explaination: number is converted to string and concatenated

B. '3' - 2 --> 1

Explaination: string is converted to number

C. 3 + null --> 3

Explaination: null becomes 0

D. '3' + null --> '3null'

Explaination: null becomes string

E. true + 3 --> 4

Explaination: true becomes 1

F. false + null --> 0

Explaination: false --> 0, null --> 0

G. '3' + undefined --> '3undefined'

Explaination: undefined becomes string

H. '3' - undefined --> NaN

Explaination: undefined becomes NaN

14. Comparison

A. '2' > 1 --> true

Explaination: '2' is converted to number 2, and 2 > 1 is true.

B. '2' < '12' --> false
Explaination: both are strings so the comparison is lexicographical. '2' comes after '1' so it is false.

C. 2 == '2' --> true
Explaination: '2' is converted to number 2 

D. 2 === '2' --> false
Explaination: === checks both value and type and these are different

E. true == 2 --> false
Explaination: true becomes 1, so 1 == 2 is false

F. true == Boolean(2) --> true
Explaination: Boolean(2) is true, and both sides are boolean

15. Differences between == and ===
== allows type coercion before comparison
=== requires both operations to be same type and value

17. The function returns:
[2, 4, 6]

Explaination: modifyArray loops through the array [1, 2, 3] and calls function doSomething to each element. doSomething multiplies each number by 2, so the result is [2, 4, 6].

19. The output is:
1
4
3
2

Explaination: 1 and 4 are printed immediately. The setTimeout with 0ms is placed in the event queue and runs after the current code finishes and 3 prints next. The setTimeout with 1000ms runs last after 1 second printing 2.