# Software design

## Clean code

### What does clean code mean?

> It means, that our code complies to the DRY and SOLID principles.

### What steps do we usually do during a clean code refactoring?

> DRY, SOLID, meaningful names

## Error handling

### What is exception handling?

> Exception handling is the process of responding to any unwanted or unexpected error during runtime.

### What are the basics of exception handling in Python?

> In Python, we use a ``try-except`` block for exception handling. The ``try`` block holds the code which could throw an 
> exception (unless we throw an exception deliberately) and the ``except`` block handles the various exceptions that may 
> occur. If there is a possibility for more than one exception to be thrown, we can handle multiple exceptions in one 
> except block, or we can use multiple exception blocks, one for each, especially if we want to handle each one 
> differently. We can catch a variety of exceptions that may occur with using the general ``Exception``, however it's 
> best to handle specific errors or use it for those cases where an unhandled exception is thrown.

### In which case should we catch an exception? Why?

> We should catch an exception when the possibility of an error occurring and ww can can take appropriate actions to 
> recover from it, or provide meaningful feedback to the user.

### What can/should we do with an exception in the ‘except’ block?

> We can and should log the exception, so we can take appropriate actions fixing the problem, we can terminate the 
> whole or part of the program to prevent the program from running in an inconsistent or error-prone state. 

### What does the else and finally statement do in a try-except block in Python?

> The ``else`` block can be run, when no exception is raised, and the ``finally`` block is run whether there was an 
> error or not. It is usually used for cleanup tasks or releasing resources. 