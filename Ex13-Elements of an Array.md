# Ex13 Fill the First 10 Elements of an Array with a Constant using Arrays.fill()
## DATE:11/11/25
## AIM:
To write a Java program that fills the first 10 elements of an array with a constant value using the Arrays.fill() method.
## Algorithm
1. Start the program.
2. Create an integer array of a specified size (for example, 15 elements).
3. Use the Arrays.fill() method to fill the first 10 elements of the array with a constant value
4.  Display the elements of the array after filling.
5.   Stop the program.

## Program:
```
/*
Program to fill the first 10 elements of an array with a constant value using the Arrays.fill() method.
Developed by: K Dilli babu 
Register Number:  212224110015
*/

import java.util.*;

public class FillArrayExample {
    public static void main(String[] args) {
        // Create an integer array of size 15
        int[] arr = new int[15];

        // Fill the first 10 elements with the constant value 5
        Arrays.fill(arr, 0, 10, 5);

        // Display the array elements
        System.out.println("Array elements after filling:");
        for (int i = 0; i < arr.length; i++) {
            System.out.print(arr[i] + " ");
        }
    }
}

```

## Output:
<img width="616" height="107" alt="image" src="https://github.com/user-attachments/assets/319de4b7-5d87-4c18-88a9-0f497aa2d1eb" />



## Result:
The program successfully fills the first 10 elements of the array with the constant value 5 using the Arrays.fill() method.
