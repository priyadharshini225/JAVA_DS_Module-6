# EX3 Write a program to count the number of digits in an integer.
## DATE: 09/03/26
## AIM:
To write a java program to count the number of digits in an integer.

## Algorithm
1. Start the program.
2. Read an integer from the user.
3. Define a recursive function countDigits() that counts digits by dividing the number by 10 each time.
4. Base condition: if the number is 0, return 0.
5. Recursive step: return 1 + countDigits(number / 10).
6. Display the total count of digits.
7. Stop the program. 

## Program:
```
/*
Program to to count the number of digits in an integer
Developed by: PRIYADHARSHINI S
RegisterNumber: 212223240129 
*/
import java.util.Scanner;

public class CountDigitsRecursive {
    static int countDigits(int n) {
        if (n == 0)
            return 0;
        return 1 + countDigits(n / 10);
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter an integer: ");
        int n = sc.nextInt();
        if (n == 0)
            System.out.println("Number of digits: 1");
        else
            System.out.println("Number of digits: " + countDigits(Math.abs(n)));
        sc.close();
    }
}
```

## Output:

<img width="432" height="181" alt="image" src="https://github.com/user-attachments/assets/89812de3-f964-42ce-9d0f-79a466ba4e9c" />


## Result:
Thus, the Java program to to count the number of digits in an integer is implemented successfully.
