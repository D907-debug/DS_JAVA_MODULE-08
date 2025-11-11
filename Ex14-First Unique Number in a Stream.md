# Ex14 Tracking the First Unique Number in a Stream using LinkedHashMap
## DATE:11/11/25
## AIM:
To implement a program that tracks the first unique (non-repeating) number in a stream of integers using a LinkedHashMap.

## Algorithm
1. Start the program
2. Create a LinkedHashMap to store integers as keys and their frequency (count) as values.
3. Read or define a stream of integers (array of numbers).
4. For each integer in the stream:

If the number is not already in the map, insert it with count = 1.

If it exists, increment its count by 1.
5.  After processing each element, find the first number in the LinkedHashMap with count = 1 (the first unique number).

6.   Display the current stream and the first unique number.
7.   Stop the program.

## Program:
```
/*
Program to track the first unique (non-repeating) number in a stream of integers using a LinkedHashMap.
Developed by: K Dilli babu 
Register Number:  212224110015
*/

import java.util.*;

public class FirstUniqueNumber {
    public static void main(String[] args) {
        // Stream of integers
        int[] stream = {4, 5, 6, 4, 7, 5, 8};

        // LinkedHashMap to maintain insertion order
        LinkedHashMap<Integer, Integer> map = new LinkedHashMap<>();

        // Process each number in the stream
        for (int num : stream) {
            map.put(num, map.getOrDefault(num, 0) + 1);

            // Find the first unique number
            Integer firstUnique = null;
            for (Map.Entry<Integer, Integer> entry : map.entrySet()) {
                if (entry.getValue() == 1) {
                    firstUnique = entry.getKey();
                    break;
                }
            }

            // Display current status
            System.out.println("Stream so far: " + Arrays.toString(Arrays.copyOfRange(stream, 0, Arrays.asList(stream).indexOf(num) + 1)));
            if (firstUnique != null)
                System.out.println("First unique number: " + firstUnique);
            else
                System.out.println("No unique number at this point.");
            System.out.println();
        }
    }
}

```

## Output:

<img width="620" height="525" alt="image" src="https://github.com/user-attachments/assets/c649fe81-4ae3-4252-9c6d-f4f47525bf22" />


## Result:
The program successfully tracks and returns the first unique number at any point in the integer stream using a LinkedHashMap.
