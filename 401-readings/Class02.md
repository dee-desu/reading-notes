
# Read 02 - Testing and Modules

**Unit Tests and Test-Driven Development**

Unit Tests are a snipit of code to test the input in your code and how would it behave. Hoever, Test-Driven Development is a way of thinking, were you write the tests first, before the actual code. 

**The Process of Writing Tests in Test-Driven Development**

We need to think about two main things, _AAA_ and _The Cycle_.

**AAA**; is the structure of thinking and it means Arrange, Act and Assert. Where you need to organize the data needed to execute that piece of code, this is called **Arrange**. Then you need to start the execution process and this is called **Act** and finally you need to check the result and compare it to the expexted result.

**The Cycle**; is the act of doing the actual TDD in baby steps, where you write the unit test and make it fail as there is noe feature to it yet, following, you need to write the feature and make it pass to one condition at a time, finally you need to refactor your code to make it presentable and beautiful.

---

# If name equals main

When running a python code, if the python interpreter is running that module (the source file) as the main program, it sets the special __name__ variable to have a value “__main__”. If this file is being imported from another module, __name__ will be set to the module’s name. Module’s name is available as value to __name__ global variable.

For example you wrote a program that contains a function that adds two numbers and returns the result, furthermore, assume your program also prints the result. Now you are working on a new module and you need to add two numbers, so you just imported the previous module, but when running you also get the printing feature from the previous module and you don't need it, to solve this issue you need to comment the part where printing occur in the previous module.

A better way of doing it is wrapping the whole code with an if statement (if __ __name__ __ == “__ __main__ __”) excluding the function, this way when the module is imported somewhere else, it will not run the logic it will only give you access to the functions and/or the code outside of the if statement scope

---
---

# Recursion

is The process in which a function calls itself directly or indirectly, think of it as a loop where the function keeps executing but without actually writing a loop and it is considered an algorithm type.

**Benifits of Recursion**

- Reduce the length of our code and make it easier to read and write, instead of writing a loop.
- Performing the same operations multiple times with different inputs.
- In every step, we try smaller inputs to make the problem smaller.
- Base condition is needed to stop the recursion otherwise infinite loop will occur.


---

# Python Modules and Packages: An Introduction

**Modules**

Modules refers to the act of Modular programming which is breaking a large, un wiedly programming task into a seperate, smaller, more manageable subtasks.

**Modules pros**

- **Simplicity**; break the big problem into smaller pieces focusing on solving little tasks at a time. 
- **Maintainability**; as the code is shorter it is easier to be updated.
- **Reusability**; it can be used in more than just one place, a module can be imported.
- **Scoping**; Avoid colusion between identifiers in different parts of a program.
