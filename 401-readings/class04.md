# Read 04 - FileIO & Exceptions

>## Files
* ### a file is a contiguous set of bytes used to store data. This data is organized in a specific format and can be anything as simple as a text file or as complicated as a program executable.

* ### Nowadays files are mostly composed of three main parts:

1. Header: Contains the data related to the file (Name, Size, Type,...etc) 
2. Data: The main contents of the file Written by the author.
3. End of file: end-of-file is a condition in a computer operating system where no more data can be read from a data source.
  >## in Python, a file operation takes place in the following order:
1. Open a file
2. Read or write (perform operation)
3. Close the file
  
  >## Opening Files in Python
  Python has a built-in `open()` function which returns a file object, so we can use it to read a file or even modify it.
  
  ```
>>> file = open("gintama_wiki.txt")    # open file in current directory
>>> file = open("C:/Python38/README.txt")  # specifying full path
  ```
* ### We can also choose the mode when opening a file. `r` for read, `w` for write, `a` for append to the file.
* ### As for the default text file mode is Read. On the other hand for other non-text file types binary mode is applied that returns bytes such as images or executable files.
  
| Mode | Description                                                                                                       | 
| ----------------------------- | ---------------------------------------------------------------------------------------- |
|   `r`  | Opens a file for reading. (default)                                                                               |
|   `w`  | Opens a file for writing. Creates a new file if it does not exist or truncates the file if it exists.             |
|   `x`  | Opens a file for exclusive creation. If the file already exists, the operation fails.                             |
|   `a`  | Opens a file for appending at the end of the file without truncating it. Creates a new file if it does not exist. |
|   `t`  | Opens in text mode. (default)                                                                                     |
|   `b`  | Opens in binary mode.                                                                                             |
|   `+`  | Opens a file for updating (reading and writing)                                                                   |

  * ### Unlike other languages, the character a does not imply the number 97 until it is encoded using ASCII (or other equivalent encodings).

* ### Moreover, the default encoding is platform dependent. In windows, it is cp1252 but utf-8 in Linux.

* ### So, we must not also rely on the default encoding or else our code will behave differently in different platforms.

* ### Hence, when working with files in text mode, it is highly recommended to specify the encoding type.
```
f = open("test.txt", mode='r', encoding='utf-8')
```
>## Closing Files in Python

* ### Its our responsibility to make sure to properly close an open file after finishing.
  * ### Python has a built-in `close()` function used to close opened files which frees up the resources that were tied with the file.
  * ### Python has a garbage collecter that clean up unrefrenced objects, but  we must not rely on it to close the files.
  
```
f = open("gintama_wiki.txt", encoding = 'utf-8')  
f.close()
```

>## Python Exceptions

### Exception handling is an essential part of any Python developer's job. If you know how to handle exceptions, you can execute any code you write flawlessly, without any interruption. A detailed guide for handling exceptions in Python can help refresh and revise your Python programming knowledge and suggest some ideas for exception handling. In this article, we define exception handling in Python, discuss different types of errors that can occur, explore five unique Python keywords for exception handling, provide relevant examples and list 20 built-in Python exceptions.
#
### When the code is syntactically correct, but it still results in an error because of some internal events, it is called an exception. It does not stop the execution, but it changes the normal flow of the program. These are usually logical errors that are non-fatal and recoverable by user programs. Programmers can handle exceptions at the run time through exception handling methods.

#

* ## What does handling exceptions in Python mean?
### The requirement for handling exceptions in Python arises when an error occurs that can cause the program to terminate. Errors interrupt the flow of the program at the point where they appear, so any further code stops executing. This error is called an exception. The exception has to be handled so that the interpreter can execute all the code that exists after the exception.

### Some common examples of such errors are dividing a number by zero, adding two incompatible types, trying to access a non-existent index of a sequence or accessing a file that does not exist. These scenarios are called exceptions. When the method cannot handle the exception, it gets thrown out of the main function, causing the program to terminate abruptly. It is necessary to prevent all such unexpected errors so that the program keeps running. Programmers write a special block of code that triggers automatically on detecting such errors. This is called exception handling in Python.
