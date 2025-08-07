# Concepts Notes

### Array
An array is similar to a list in Python. It is a collection of elements that are all of the same type. Each element is stored at a specific index, and all elements are grouped under one variable name.

### 🔤 String
A string is a sequence of characters. But how does a computer know where a string ends?  
In C, every string is automatically followed by a special character called the **null terminator**, written as `\0`.  
For example, the string `"HI!"` seems to use three memory blocks, but it actually takes **four**. The last block is reserved for `\0`, which is `00000000` in binary.

### 🧱 NUL vs Null
- **NUL**: A special terminating character (`\0`) that tells the computer where the string ends.  
- **Null**: A keyword that represents "no value" or "nothing". It is used to indicate that a pointer doesn't point to anything.

### 📏 String Length
To measure the length of a string in C, we use the function `strlen()`, which is declared in the header file `string.h`.  
It works similarly to Python’s `len()` function.

### 💻 Command-Line Arguments
In C, we can receive command-line input using this syntax:
```c
int main(int argc, string argv[])
argc (argument count): the number of command-line arguments.
argv (argument vector): an array of strings, each one representing a command-line argument entered by the user.

### Exit status
When a program ends, it can return a number called an exit status to indicate success or failure:
-return 0; → success
-return 1; or any non-zero value → an error or bug occurred

