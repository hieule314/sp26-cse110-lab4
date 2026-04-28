1. The bug was that num1 and num2 were being retrieved using .value, which returns strings rather than integers. This is due to the + operator to concatenate the values instead of adding them as integers.

2. I would fix it by converting the values to numbers before adding;

let result = Number(num1) + Number(num2);