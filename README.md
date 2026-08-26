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
<img width="628" height="506" alt="image" src="https://github.com/user-attachments/assets/39d3cbec-4640-4e05-8921-3e57ecb38d91" />

### Explanation:

The make_username function builds a lowercase username by cleaning up both name inputs and combining them with a period. The order of the two characters within the string is maintained, each letter's transformed to lowercase by utilizing the .lower() code.

### C. BOOKEND SWAP PROBLEM
Swapping boundary elements of a list requires isolating the first and last elements while leaving the middle elements untouched and preserving the original list structure.

* `first, *middle, last = items` - extracts index `0` into `first`, index `-1` into `last`, and all intermediate elements into `middle` as a list.

* `[last] + middle + [first]` - reconstructs a new list with swapped boundaries.

* `*middle` - capture excess iterable items into a dynamic sublist.

  *Example: `a, *b, c = [10, 20, 30, 40]` assigns a=[10], b=[20, 30], c=[40]*

* `+` - Combines list instances into a new list instance without altering inputs.
  *Example: `[1] + [2, 3] + [4] = [1, 2, 3, 4]`*
