# EX3 Write a program to count the number of digits in an integer.
## DATE: 16/07/2026
## AIM:
To write a C program to implement Tower of Hanoi

## Algorithma

1. Read the input number Take an integer num from the user.
2. Convert the number to a non-negative value Use Math.abs(num) and store it in n to handle negative numbers.
3. Check if the number is zero If n == 0, set digit count to 1 (since zero has one digit).
4. Count digits for non-zero numbers Repeatedly divide n by 10 and increment the counter until n becomes 0.
5. Display the digit count Output the total number of digits.
    
## Program:
```java
/*
Program to to count the number of digits in an integer
Developed by: HARSHADA P K
RegisterNumber: 212224060097
*/

import java.util.Scanner;

public class CountDigits {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int num = sc.nextInt();

        int count = 0;
        int n = Math.abs(num); 

        if (n == 0) {
            count = 1; 
        } else {
            while (n > 0) {
                n /= 10; 
                count++;
            }
        }

        System.out.println("Number of digits: " + count);
    }
}
```

## Output:
<img width="733" height="328" alt="01" src="https://github.com/user-attachments/assets/912ff986-b3d6-4ddf-ad81-ae28ea3a19f5" />


## Result:
Thus, the Java program to to count the number of digits in an integer is implemented successfully.
