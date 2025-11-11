# Ex12 Add Elements from an Array into a TreeSet
## DATE:11/11/25
## AIM:
To write a Java program that adds elements from an array into a TreeSet and displays the elements in sorted order.
## Algorithm
1. Start the program.
2. Create an array containing a few integer elements.
3. Create a TreeSet to store elements in sorted order.
4.  Use a loop to add each element of the array into the TreeSet.
5.   Display the elements of the TreeSet.
6.   Stop the program.

## Program:
```
/*
Program that adds elements from an array into a TreeSet and displays the elements in sorted order.
Developed by: K Dilli babu
Register Number:  212224110015
*/

import java.util.*;

public class ArrayToTreeSet {
    public static void main(String[] args) {
        // Create an array of integers
        Integer[] numbers = {50, 10, 30, 20, 40};

        // Create a TreeSet
        TreeSet<Integer> treeSet = new TreeSet<Integer>();

        // Add elements from the array into the TreeSet
        for (int num : numbers) {
            treeSet.add(num);
        }

        // Display elements of TreeSet
        System.out.println("Elements of the TreeSet in sorted order: " + treeSet);
    }
}

```

## Output:

<img width="593" height="95" alt="image" src="https://github.com/user-attachments/assets/8773d94a-ff2a-4205-8a6a-135430c05818" />


## Result:
The program successfully adds elements from an array into a TreeSet.
