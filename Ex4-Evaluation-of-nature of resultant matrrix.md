# Ex4 : You are given a Java program that performs matrix addition. If Matrix A has all odd numbers and Matrix B has all even numbers of the same dimension, what will be the nature (even/odd/mixed) of the resulting matrix?

## DATE: 20/09/2026

## AIM:

To write a Java function to evaluate whether the given Matrix A has all odd numbers and Matrix B has all even numbers of the same dimension and find the nature of resultant matrix.

## Algorithm

1. Read the dimensions and elements of Matrix A and Matrix B.
2. Add the corresponding elements of Matrix A and Matrix B.
3. Check whether each element of the resultant matrix is even or odd.
4. Since odd + even always produces an odd number, identify the resultant matrix as odd.
5. Display the resultant matrix and its nature.

## Program:

```java
/*
Program to find the nature of resultant matrix.
Developed by: LAKSHMIDHAR N
RegisterNumber:  212224230138
*/

import java.util.*;

public class Main {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int rows = sc.nextInt();
        int cols = sc.nextInt();

        int[][] A = new int[rows][cols];
        int[][] B = new int[rows][cols];
        int[][] result = new int[rows][cols];

        for (int i = 0; i < rows; i++)
            for (int j = 0; j < cols; j++)
                A[i][j] = sc.nextInt();

        for (int i = 0; i < rows; i++)
            for (int j = 0; j < cols; j++)
                B[i][j] = sc.nextInt();

        for (int i = 0; i < rows; i++) {
            for (int j = 0; j < cols; j++) {
                result[i][j] = A[i][j] + B[i][j];
            }
        }

        for (int i = 0; i < rows; i++) {
            for (int j = 0; j < cols; j++)
                System.out.print(result[i][j] + " ");
            System.out.println();
        }

        System.out.println("Nature: Odd");
    }
}
```

## Output:

<img width="435" height="221" alt="image" src="https://github.com/user-attachments/assets/fea25a9d-fc96-4d18-b304-95c6d44b64f5" />


## Result:

Thus, the Java program to evaluate whether the given Matrix A has all odd numbers and Matrix B has all even numbers of the same dimension and find the nature of resultant matrix is implemented successfully.
