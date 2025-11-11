# Ex15 Value Existence Check in a TreeMap
## DATE:11/11/25
## AIM:
To write a Java program that checks whether a given value exists in a TreeMap.

## Algorithm
1. Start the program.
2. Create a TreeMap to store key–value pairs.
3. Insert some sample key–value pairs into the TreeMap.
4. Display the contents of the TreeMap.
5. Use the containsValue() method to check whether a specific value exists in the map.
6.  Display the result based on the check.
7.   Stop the program.

## Program:
```
/*
Program to check whether a given value exists in a TreeMap.
Developed by: K Dilli babu
Register Number:  212224110015
*/

import java.util.*;

public class ValueExistenceCheck {
    public static void main(String[] args) {
        // Create a TreeMap
        TreeMap<Integer, String> map = new TreeMap<Integer, String>();

        // Add key-value pairs
        map.put(1, "Apple");
        map.put(2, "Banana");
        map.put(3, "Cherry");
        map.put(4, "Mango");
        map.put(5, "Orange");

        // Display the TreeMap
        System.out.println("TreeMap Elements: " + map);

        // Value to check
        String valueToCheck = "Mango";

        // Check if the value exists
        if (map.containsValue(valueToCheck)) {
            System.out.println("The value \"" + valueToCheck + "\" exists in the TreeMap.");
        } else {
            System.out.println("The value \"" + valueToCheck + "\" does not exist in the TreeMap.");
        }
    }
}

```

## Output:

<img width="671" height="129" alt="image" src="https://github.com/user-attachments/assets/66e53c81-7b65-4eb5-b3be-69db9f41c903" />


## Result:
Thus, the program successfully checks whether a specified value exists in a TreeMap using the containsValue() method.
