# EX3 : Write a program to count the number of digits in an integer.

## DATE: 20/09/2026

## AIM:

To write a Java program to count the number of digits in an integer.

## Algorithm

1. Read an integer from the user.
2. Create a recursive method to count the digits.
3. If the number is less than 10, return 1.
4. Divide the number by 10 and recursively count the remaining digits.
5. Print the total number of digits.

## Program:

```java
/*
Program to count the number of digits in an integer
Developed by: LAKSHMIDHAR N
RegisterNumber:  212224230138
*/

import java.util.*;

public class Main {

    static int countDigits(int n) {
        n = Math.abs(n);

        if (n < 10)
            return 1;

        return 1 + countDigits(n / 10);
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int n = sc.nextInt();

        System.out.println(countDigits(n));
    }
}
```

## Output:

<img width="207" height="58" alt="image" src="https://github.com/user-attachments/assets/30a397b6-5822-43bd-b642-0896c450de7f" />


## Result:

Thus, the Java program to count the number of digits in an integer is implemented successfully.

