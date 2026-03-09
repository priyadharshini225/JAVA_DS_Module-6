# Ex4 You are given a Java program that performs matrix addition. If Matrix A has all odd numbers and Matrix B has all even numbers of the same dimension, what will be the nature (even/odd/mixed) of the resulting matrix?
## DATE: 09/03/26
## AIM:
To write a java function to evaluate weather the given Matrix A has all odd numbers and Matrix B has all even numbers of the same dimension and find the nature of resultant matrrix.

## Algorithm
1. Start the program and read the number of rows and columns of Matrix A and Matrix B.
2. Check dimensions of both matrices. If they are not equal, display “Matrices are not of same dimension” and stop.
3. Read Matrix A and check elements. If any element is even, mark Matrix A as invalid and stop.
4. Compute the resultant matrix (e.g., A + B) if matrices are valid.
5. Check resultant matrix: if all elements are odd print “Odd Matrix”, if all are even print “Even Matrix”, then display the matrix and stop.

## Program:
```
/*
Program to ind the nature of resultant matrrix.
Developed by: PRIYADHARSHINI S
RegisterNumber: 212223240129 
*/
import java.util.Scanner;

public class MatrixAddition {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int rows = sc.nextInt();
        int cols = sc.nextInt();

        int[][] A = new int[rows][cols];
        int[][] B = new int[rows][cols];
        int[][] result = new int[rows][cols];

        for (int i = 0; i < rows; i++) {
            for (int j = 0; j < cols; j++) {
                A[i][j] = sc.nextInt();
            }
        }
        for (int i = 0; i < rows; i++) {
            for (int j = 0; j < cols; j++) {
                B[i][j] = sc.nextInt();
            }
        }
        for (int i = 0; i < rows; i++) {
            for (int j = 0; j < cols; j++) {
                result[i][j] = A[i][j] + B[i][j];
            }
        }
        for (int i = 0; i < rows; i++) {
            for (int j = 0; j < cols; j++) {
                System.out.print(result[i][j] + " ");
            }
            System.out.println();
        }

       
    }
}
```

## Output:

<img width="524" height="766" alt="image" src="https://github.com/user-attachments/assets/1a377cee-0045-406d-aac3-a0b72d2cf04c" />


## Result:
Thus, the java program to evaluate weather the given Matrix A has all odd numbers and Matrix B has all even numbers of the same dimension and find the nature of resultant matrrix is implemented successfully.
