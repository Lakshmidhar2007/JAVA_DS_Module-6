# Ex2 : Count how many times a number appears in an array recursively.

## DATE: 20/09/2026

## AIM:

To write a Java program to Count how many times a number appears in an array recursively.

## Algorithm

1. Read the number of elements and store them in an array.
2. Read the number whose occurrences need to be counted.
3. Create a recursive method to check each array element.
4. If the current element matches the target number, increase the count and recursively check the remaining elements.
5. Print the total number of occurrences.

## Program:

```java
/*
Program Count how many times a number appears in an array recursively.
Developed by: LAKSHMIDHAR N
RegisterNumber:  212224230138
*/

import java.util.*;

public class Main {

    static int countOccurrences(int[] arr, int n, int target) {
        if (n == 0)
            return 0;

        return (arr[n - 1] == target ? 1 : 0)
                + countOccurrences(arr, n - 1, target);
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int n = sc.nextInt();
        int[] arr = new int[n];

        for (int i = 0; i < n; i++)
            arr[i] = sc.nextInt();

        int target = sc.nextInt();

        System.out.println(countOccurrences(arr, n, target));
    }
}
```

## Output:

<img width="197" height="97" alt="image" src="https://github.com/user-attachments/assets/c06aa125-1e7d-4b9a-b7fa-4df71cec8a06" />


## Result:

Thus, the Java program to Count how many times a number appears in an array recursively is implemented successfully.
