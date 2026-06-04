evaulate exp cmd 
expr 30 + 10 
expr 30 - 10
expr 30 / 10 
expr 30 * 10 -> in bash "*" means "everything" it's not used for multi. 
expr 30 \* 10 -> this will work for multiplication
expr 30 % 10 -> modulo (remainder)
expr 30 > 10 -> comparison (returns 1 for true, 0 for false)
expr 30 = 30 -> equality check

double parentheses for math:
echo $((5 + 5))
echo $((10 - 3))
echo $((4 * 5))
echo $((20 / 4))
echo $((20 % 3)) -> modulo operator

let command:
let x=10+5
echo $x -> output: 15
let "y = 30 * 2"
echo $y -> output: 60

bc command (calculator):
echo "5.5 + 3.2" | bc
echo "scale=2; 10/3" | bc -> scale sets decimal places

integer comparison:
-eq (equal)
-ne (not equal)
-lt (less than)
-gt (greater than)
-le (less than or equal)
-ge (greater than or equal)  

