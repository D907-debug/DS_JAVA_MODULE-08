# Ex11 Convert HashSet to ArrayList in Java
## DATE:11/11/25
## AIM:
To convert a collection of distinct integers stored in a HashSet into an ArrayList and display its contents.
## Algorithm
1. Start the program.
2. Create a HashSet to store a collection of distinct integers.
3. Add a few integers to the HashSet.
4.  Create an ArrayList and initialize it with the elements of the HashSet.
5.  Display the elements of both HashSet and ArrayList.
6.   Stop the program.

## Program:
```
/*
Program to convert a collection of distinct integers stored in a HashSet into an ArrayList and display its contents.
Developed by: K Dilli babu 
Register Number:  212224110015
*/

import java.util.*;

public class HashSetToArrayList {
    public static void main(String[] args) {
        // Create a HashSet
        HashSet<Integer> set = new HashSet<Integer>();
        set.add(10);
        set.add(20);
        set.add(30);
        set.add(40);
        set.add(50);

        System.out.println("HashSet elements: " + set);

        // Convert HashSet to ArrayList
        ArrayList<Integer> list = new ArrayList<Integer>(set);

        // Display ArrayList elements
        System.out.println("ArrayList elements: " + list);
    }
}

```

## Output:

<img width="601" height="122" alt="image" src="https://github.com/user-attachments/assets/e0c71739-477a-450d-ba79-cbeecf24e8c0" />


## Result:
The program successfully converts a collection of distinct integers stored in a HashSet into an ArrayList
