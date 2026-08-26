# ECE2112 PA 1
### OBJECTIVE
To implement fundamental Python concepts such as string slicing, string methods and extended sequence unpacking
by creating functions in Jupyter Notebook

### A. WORD ROTATION PROBLEM
A string rotation involves shifting characters along a sequence without changing their relative orders.
In this problem, the operation only moves the beginning and end of the string.

* `rotate_word(text)` - accesses string elements using sequence slicing.
  
* `text[1:]` - extracts a substring containing everything from index `1`. It continues up to the end of the string because of the symbol `:`, which mean "from this position to the end".

	*Example: `"hello"[1:] = "ello"`*

	It extracted from index `1` ("e") up to the end of the string.

* `text[0]` - targets the single character at index `0`.

  *Example: `"hello"[0] = "h"`*

	It extracted only index `0` ("h")

Combining these expressions (`text[1:] + text[0]`) effectively places the first character at the end of the string, forming the rotated word.

*Example: `rotate_word("hello") = "elloh"`*

<img width="1189" height="158" alt="Screenshot 2026-08-23 085209" src="https://github.com/user-attachments/assets/9ace0acc-6d1b-4959-a09c-797bcd456fa3" />

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
