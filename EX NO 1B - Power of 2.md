
# EX 1B Power of 2
## DATE:
## AIM:
To write a Java program to for given constraints.Given an integer n, return true if it is a power of two. Otherwise, return false.

An integer n is a power of two, if there exists an integer x such that n == 2x.

## Algorithm
1. Start
2. Read an integer n from the user.
3. Check whether n is positive and repeatedly divide n by 2 while it is divisible by 2.
4. If the final value of n is 1, print true; otherwise, print false.
5. Stop

## Program:
```
/*
Program to implement Reverse a String :

import java.util.Scanner;
public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        if (n > 0 && (n & (n - 1)) == 0) {
            System.out.println("true");
        } else {
            System.out.println("false");
        }
    }
}
Developed by: ibrahim fedah s
Register Number: 212223240056
*/
```

## Output:

<img width="1028" height="283" alt="image" src="https://github.com/user-attachments/assets/c5382bbf-da7c-4c8c-abe9-6c961d711828" />


## Result:
The program successfully implemented and the expected output is verified.
