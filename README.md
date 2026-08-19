# CSCE 10204: Foundations fo Programming II - PreCourse Review Assignment

**Instructions:** Write complete Java code solutions for each of the following questions. Observe all specified restrictions, including manual index-based string processing, explicit exception handling, and proper resource management.

---

### **Problem 1: Arrays**

Write a complete static method named `findMaxDifference` that accepts an array of integers (`int[] numbers`) as its parameter and returns an `int`. The method should calculate and return the maximum absolute difference between any two adjacent elements in the array.

- **Requirements:**
  - If the array has fewer than 2 elements, return `0`.
  - Do not sort or alter the original array.
  - Use array indexing and length checks appropriately.

- **Example:**
  Given `{4, 7, 2, 9, 1}`:
  - Difference between `4` and `7` = $|4 - 7| = 3$
  - Difference between `7` and `2` = $|7 - 2| = 5$
  - Difference between `2` and `9` = $|2 - 9| = 7$
  - Difference between `9` and `1` = $|9 - 1| = 8$
  - **Return:** `8`

---

### **Problem 2: String Processing (Character at a Time)**

Write a complete static method named `countVowelSequences` that takes a `String str` as a parameter and returns an `int`. The method must process the string character-by-character using a manual loop and `charAt()` to count how many times two vowels appear sequentially next to each other. You cannot use any methods from the `String` class except for `charAt()` and `equals()`.

- **Requirements:**
  - Vowels are `'a'`, `'e'`, `'i'`, `'o'`, `'u'` (case-insensitive).
  - You **may not** use `String.split()`, regular expressions, or `toCharArray()`. You must iterate using string indices and bounds checking.

- **Example:**
  Given `"Steam engine in heavy rain"`:
  - Vowel sequences found: `"ea"` in _Steam_, `"ea"` in _heavy_, and `"ai"` in _rain_.
  - **Return:** `3`

---

### **Problem 3: Basic Text File I/O**

Write a complete static method named `filterLogFile` that takes two string parameters: `String inputFileName` and `String outputFileName`. The method must read lines from the input file and write only lines that begin with the prefix `"[ERROR]"` to the output file using `Scanner` and `PrintWriter`.

- **Requirements:**
  - Explicitly declare checked exceptions on the method signature using `throws IOException`.
  - Ensure file resources (`Scanner` and `PrintWriter`) are properly closed.
  - Write each qualifying line to the output file on a new line.
