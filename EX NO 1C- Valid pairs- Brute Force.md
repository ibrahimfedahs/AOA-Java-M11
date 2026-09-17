
# EX 1C Valid Pairs using Brute Force Approach
## DATE:
## AIM:
To write a Java program to for given constraints.
Given an integer array nums and an integer k, return the number of pairs (i, j) where i < j such that |nums[i] - nums[j]| == k.

The value of |x| is defined as:

x if x >= 0.
-x if x < 0.

## Algorithm
1. Start
2. Read the size of the array, the array elements, and the value of k.
3. Initialize count = 0.
4. Compare every pair of elements where i < j. If |nums[i] - nums[j]| == k, increment count.
5. Print count and Stop. 

## Program:
```
/*
Program to implement Reverse a String :

import java.util.Scanner;
public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int[] nums = new int[n];
        for (int i = 0; i < n; i++) {
            nums[i] = sc.nextInt();
        }
        int k = sc.nextInt();
        int count = 0;
        for (int i = 0; i < n; i++) {
            for (int j = i + 1; j < n; j++) {
                if (Math.abs(nums[i] - nums[j]) == k) {
                    count++;
                }
            }
        }
        System.out.println(count);
    }
}
Developed by: ibrahim fedah s
Register Number: 212223240056
*/
```

## Output:

<img width="1025" height="359" alt="image" src="https://github.com/user-attachments/assets/61106ebd-2297-4575-8471-1c547b37f011" />


## Result:
The program successfully implemented and the expected output is verified.
