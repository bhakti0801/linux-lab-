# LAB 3 – Enhanced Number Script

---

## 🧾 Original Behavior
![alt text](image-27.png)

### Explanation:
📥 User input collection
These read commands take input from the user:

start: the beginning of the number range

end: the maximum value to count to

step: how much to increase each time

✅ Step validation

"$step" =~ ^[0-9]+$ → Ensures the input contains only digits (i.e., it's a number).

"$step" -le 0 → Checks if the number is less than or equal to zero.

If either check fails, the script shows an error and exits.

🔁 C-style for loop

Starts from i = start

Loops until i <= end

Increments i by step in each iteration

💬 Output inside loop

Prints the current number in the loop.

Loop continues based on step.
### OUTPUT:
![alt text](image-28.png)
### Script: `print_numbers.sh`
- Printed numbers from 1 to 5 using a hardcoded `for` loop:
```bash
for i in 1 2 3 4 5
do
  echo "Number: $i"
done
Q 1 Difference between $1, $@, and $# in bash?
A1  The difference between $1, $@ and $# is:
•	$1- Takes the first argument.
•	$@- Takes all the argument but separately. 
•	$#- Number of arguments
Q2 What does exit 1 mean in a script?
A2
•	To stop execution when an error is detected.
•	To inform other programs or scripts that this script failed or encountered a problem.


