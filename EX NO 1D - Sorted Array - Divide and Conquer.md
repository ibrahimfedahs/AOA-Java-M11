
# EX 1D Sorted Array using Divide and Conquer Approach.
## DATE:
## AIM:
To write a Java program to for given constraints.
Given two sorted arrays nums1 and nums2 of size m and n respectively, return the median of the two sorted arrays.

The overall run time complexity should be O(log (m+n)).

## Algorithm
1. Start
2. Read the sizes and elements of the two sorted arrays.
3. Perform binary search on the smaller array and find a partition such that all elements on the left are smaller than all elements on the right.
4. Calculate the median based on the total number of elements. If the total is even, take the average of the two middle elements.
5. Print the median and Stop.

## Program:
```
/*
Program to Find Median of Two Sorted Arrays:

import java.util.Scanner;

public class Main {

    public static double findMedian(int[] nums1, int[] nums2) {

        if (nums1.length > nums2.length) {
            int[] temp = nums1;
            nums1 = nums2;
            nums2 = temp;
        }

        int m = nums1.length;
        int n = nums2.length;

        int low = 0, high = m;

        while (low <= high) {
            int partition1 = (low + high) / 2;
            int partition2 = (m + n + 1) / 2 - partition1;

            int left1 = (partition1 == 0) ? Integer.MIN_VALUE : nums1[partition1 - 1];
            int right1 = (partition1 == m) ? Integer.MAX_VALUE : nums1[partition1];

            int left2 = (partition2 == 0) ? Integer.MIN_VALUE : nums2[partition2 - 1];
            int right2 = (partition2 == n) ? Integer.MAX_VALUE : nums2[partition2];

            if (left1 <= right2 && left2 <= right1) {

                if ((m + n) % 2 == 0) {
                    return (Math.max(left1, left2) +
                            Math.min(right1, right2)) / 2.0;
                } else {
                    return Math.max(left1, left2);
                }

            } else if (left1 > right2) {
                high = partition1 - 1;
            } else {
                low = partition1 + 1;
            }
        }

        return 0.0;
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int m = sc.nextInt();
        int[] nums1 = new int[m];

        for (int i = 0; i < m; i++) {
            nums1[i] = sc.nextInt();
        }

        int n = sc.nextInt();
        int[] nums2 = new int[n];

        for (int i = 0; i < n; i++) {
            nums2[i] = sc.nextInt();
        }

        System.out.println(findMedian(nums1, nums2));
    }
}
Developed by: ibrahim fedah s
Register Number: 212223240056

*/
```

## Output:
<img width="1023" height="401" alt="image" src="https://github.com/user-attachments/assets/40b079b7-25b5-4360-a94b-57ccbf6898b1" />



## Result:
The program successfully implemented and the expected output is verified.
