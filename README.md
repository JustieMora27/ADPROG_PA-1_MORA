# ECE2112 PA 1
## Instructions
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


### -----------------------------------------------------------------------------------------------------------------------------


### B. USERNAME BUILDER PROBLEM
<img width="628" height="506" alt="image" src="https://github.com/user-attachments/assets/39d3cbec-4640-4e05-8921-3e57ecb38d91" />

### Explanation:

The make_username function builds a lowercase username by cleaning up both name inputs and combining them with a period. The order of the two characters within the string is maintained, each letter's transformed to lowercase by utilizing the .lower() code. For example, the string Lebron James' order of letters is maintained however, all letters are now lowercase and are separated by a period instead.


### -----------------------------------------------------------------------------------------------------------------------------


### C. BOOKEND SWAP PROBLEM
<img width="655" height="476" alt="image" src="https://github.com/user-attachments/assets/b51b232f-aa19-4e88-9465-0f9653bc8d89" />

### Explanation:

The swap_bookends function swaps the first and last items of a list while keeping all middle items in their original order. For example, in 1 to 6, only 1 and 6 swapped places, the rest of them didn't switch. So if you only have 2 characters then they are simply going to switch.

