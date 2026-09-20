# Ex5 : Count Inversions in an Array

## DATE: 20/09/2026

## AIM:

To write a Java program to Count the number of inversions in an array where inversion is defined as: arr[i] > arr[j] and i < j

## Algorithm

1. Read the number of elements and store them in an array.
2. Create a recursive method to compare each element with the elements after it.
3. If `arr[i] > arr[j]` and `i < j`, count it as an inversion.
4. Recursively check all possible pairs in the array.
5. Print the total number of inversions.

## Program:

```java
/*
Program to Count the number of inversions in an array where inversion is defined as: arr[i] > arr[j] and i < j
Developed by: LAKSHMIDHAR N
RegisterNumber:  212224230138
*/

import java.util.*;

public class Main {

    static int countInversions(int[] arr, int i, int j) {
        if (i >= arr.length - 1)
            return 0;

        if (j >= arr.length)
            return countInversions(arr, i + 1, i + 2);

        int count = (arr[i] > arr[j]) ? 1 : 0;

        return count + countInversions(arr, i, j + 1);
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int n = sc.nextInt();
        int[] arr = new int[n];

        for (int i = 0; i < n; i++)
            arr[i] = sc.nextInt();

        System.out.println(countInversions(arr, 0, 1));
    }
}
```

## Output:

<img width="608" height="155" alt="image" src="https://github.com/user-attachments/assets/5370cc84-2f16-41fd-b0ce-225e710a279d" />


## Result:

Thus the Java program to Count the number of inversions in an array where inversion is defined as: arr[i] > arr[j] and i < j is implemented successfully.
