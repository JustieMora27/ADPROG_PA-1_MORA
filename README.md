# ECE2112 PA 1
### Instructions
Write a Python program in a Jupyter Notebook to solve each of the following problems.

• Use the exact function names specified in each problem.

•Place each problem in a separate, clearly labeled section of the notebook.

• Each function must return the required result unless printed output is explicitly requested.

• Do not use external Python libraries.

• Use only basic Python operations, string methods, slicing, and sequence unpacking. Loops and
classes are not required.

• Test each function using the examples provided. Additional valid inputs may be used when grading
the notebook.

### -----------------------------------------------------------------------------------------------------------------------------

### A. WORD ROTATION PROBLEM
<img width="493" height="561" alt="image" src="https://github.com/user-attachments/assets/6ced1e82-f124-4f21-8ce6-8acc3997c014" />

### Explanation:

What The rotate_word function does is it moves the first character of a string to the end using string slicing while maintaining the capitalization of that specific letter. For example, we have Justie. It starts with the letter J and is capitalized. After running the code, the capitalized letter J will go at the end of the string, which gives us ustieJ.

### B. USERNAME BUILDER PROBLEM
Generating standardized user inputs requires cleaning up formatting discrepancies such as mixed capitalizations and removing spaces across multiple word inputs before combining them.

* `.lower()` - converts all uppercase characters acroos both input strings to lowercase to ensure consistency.

	*Example: `"John".lower() = "john"`*
  
* `.replace(" ", "")` - replaces every space characters with an empty string, effectively removing all spaces wether they occur between words or at boundaries.

  *Example: `"De Leon".replace(" ", "") = "DeLeon"`*
  
* `+ "." +` - joins the processed strings using a period as a connector

	*Example: `"ana" + "." + "maria" = "ana.maria"`*

<img width="1189" height="223" alt="image" src="https://github.com/user-attachments/assets/f0a6ae7c-2e63-405c-a996-d382793f5e12" />

### C. BOOKEND SWAP PROBLEM
Swapping boundary elements of a list requires isolating the first and last elements while leaving the middle elements untouched and preserving the original list structure.

* `first, *middle, last = items` - extracts index `0` into `first`, index `-1` into `last`, and all intermediate elements into `middle` as a list.

* `[last] + middle + [first]` - reconstructs a new list with swapped boundaries.

* `*middle` - capture excess iterable items into a dynamic sublist.

  *Example: `a, *b, c = [10, 20, 30, 40]` assigns a=[10], b=[20, 30], c=[40]*

* `+` - Combines list instances into a new list instance without altering inputs.
  *Example: `[1] + [2, 3] + [4] = [1, 2, 3, 4]`*
