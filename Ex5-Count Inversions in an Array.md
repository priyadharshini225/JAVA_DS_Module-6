# Ex5 Count Inversions in an Array
## DATE: 09/03/26
## AIM:
To write a Java program  to Count the number of inversions in an array where inversion is defined as: arr[i] > arr[j] and i < j

## Algorithm
1. Start the program and read the number of elements n.
2. Declare an array arr and read n elements into the array.
3. Initialize a variable count = 0 to store the number of inversions.
4. Use two nested loops to compare elements and if arr[i] > arr[j], increment count.
5. Display the inversion count and stop the program.

## Program:
```
/*
Program toto Count the number of inversions in an array where inversion is defined as: arr[i] > arr[j] and i < j
Developed by: PRIYADHARSHINI S 
RegisterNumber: 212223240129
*/
import java.util.Scanner;

public class CountInversions
{
    public static int countInversions(int[] arr)
{
        int n = arr.length;
        int count = 0;
        for (int i = 0; i < n - 1; i++)
{
            for (int j = i + 1; j < n; j++)
{
                if (arr[i] > arr[j]) {
                    count++; 
                }
            }
        }

        return count;
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter number of elements: ");
        int n = sc.nextInt();

        int[] arr = new int[n];

        System.out.println("Enter " + n + " elements:");
        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }

        int inversions = countInversions(arr);

        System.out.println("Number of inversions in the array: " + inversions);

        sc.close();
    }
}
```

## Output:

<img width="457" height="229" alt="image" src="https://github.com/user-attachments/assets/5bd04487-429b-4ee1-8cea-a1a26c72a03e" />


## Result:
Thus the Java program to to Count the number of inversions in an array where inversion is defined as: arr[i] > arr[j] and i < jis implemented successfully.
