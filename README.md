# Investigating Pauses in Writing Code using Codeitz, a Personalized Programming Tutor

Programmers who exhibited self-regulated programming techniques paused to consider alternate approaches, revisit requirements, or think about which programming concepts to use. Additionally, we found patterns in burst sizes for different types of exercises.

### WS_CI_1

Consider the class:

```java
public class Employee {
    int role;
    float salary;
}
```

Write code to
1. Create a method `verifyEmployee` that takes parameters `Employee e1` and `Employee e2`
2. Write a statement that returns a `-1` if e1’s role is less than e2’s and e1’s salary is also less than e2’s.
3. Write another statement that returns `0` if `e1` and `e2` have the same roles and salaries.
4. Write another statement that returns a `1` if e1’s role is greater than e2’s and e1’s salary is also greater than e2’s.
5. Write a final line that returns a `2` if none of the previous rules could be verified.

Write your code below.

### WS_CI_2
The following method returns `0` if `x` is not divisible by `n` and `1` if `x` is divisible by `n`.

``` java
public static int xIsDivisibleByN(int x, int n) {
    if (x % n == 0) {
        return 1;
    } else {
        return 0;
    }
}
```

Create a program that asks the user to input a number and uses the method `xIsDivisibleByN` to determine if it is prime, that is, if it is divisible by no number except itself and `1`. Assume that the user will input an integer greater than or equal to `2`.

Follow the steps below to create your code:
1.	Write a statement to import `java.util.Scanner`
2.	Declare a public class "Main".
Within the `Main` class, do the following:
3.	Declare a public static method `main` which does not return anything and takes as a parameter an array of Strings named `args`.

Within the main method, do the following:

4.	Declare an integer variable named `a`.
5.	Define a new Scanner object `sc` which takes `System.in` as a parameter.
6.	Set a to the returned value of Scanner sc's `nextInt()` method.
7.	Declare an integer `isPrime` and set it to `1`.
8.	Declare an integer variable `root` and set it to the square root of a casted as an integer.
9.	Create a for loop that uses integer variable n to go from `2` to `root` (inclusive), incrementally increasing by `1`.
Inside that for loop, do the following:
10.	Set `isPrime` to the value returned by passing `a` and `n` into the `xIsDivisibleByN` method.
11.	If `isPrime` to `0`, break out of the for loop.

Outside of the for loop, do the following:

12.	If `isPrime` is equal to `1`, print the formatted string "Number {num} is prime"  (where {num} the value stored in a)
13.	If the if statement is not true, print the formatted string "Number {num} is NOT prime"  (where {num} the value stored in a)

