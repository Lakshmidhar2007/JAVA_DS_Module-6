# EX 1 You’re creating a health monitoring device which stores several sensor readings in an array. To determine the minimum value (e.g., lowest heartbeat), implement a recursive method.
## DATE: 20/09/2026
## AIM:
To write a JAVA program To determine the minimum value (e.g., lowest heartbeat), implement a recursive method.

## Algorithm
1. Read the number of elements and store them in an array.
2. Create a recursive method to find the minimum value.
3. If only one element remains, return that element.
4. Recursively find the minimum of the remaining elements and compare it with the current element.
5. Print the minimum value.

## Program:
```

Program To determine the minimum value (e.g., lowest heartbeat), implement a recursive method.
Developed by: LAKSHMIDHAR N
RegisterNumber:  212224230138

```
```java
import java.util.*;

public class Main {

    static int findMin(int[] arr, int n) {
        if (n == 1)
            return arr[0];

        return Math.min(arr[n - 1], findMin(arr, n - 1));
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int n = sc.nextInt();
        int[] arr = new int[n];

        for (int i = 0; i < n; i++)
            arr[i] = sc.nextInt();

        System.out.println(findMin(arr, n));
    }
}
```
## Output:
<img width="236" height="83" alt="image" src="https://github.com/user-attachments/assets/6f159f81-f107-4ba3-8d50-18147533aff6" />



## Result:
Thus the Java program to find the minimum value (e.g., lowest heartbeat), implement a recursive method has implemented successfully
