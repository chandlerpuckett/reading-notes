# The Call Stack & Debugging

## CHEATSHEET

> a **call stack** is a mechanism for an interpreter to keep track of its place in a script that calls multiple functions -- what function is currently being run and what functions are called from within that function

- When a script calls a function, the interpreter adds it to the call stack and then starts carrying out the function.
- Any functions that are called by that function are added to the call stack further up, and run where their calls are reached.
- When the current function is finished, the interpreter takes it off the stack and resumes execution where it left off in the last code listing.
- If the stack takes up more space than it had assigned to it, it results in a "stack overflow" error.

- we start with an empty call stack
- invoking adds a function to the call stack
- after execution, it is automatically removed

- JS is a single threaded interpreter 

#### The understanding of the call stack is vital to Asynchronous programming

- In Asynchronous JavaScript, we have a callback function, an event loop, and a task queue.
  - The callback function is acted upon by the call stack during execution after the call back function has been pushed to the stack by the event loop

#### This is what happens when the code is run:

1. When `secondFunction()` gets executed, an empty stack frame is created. It is the main (anonymous) entry point of the program.
2. `secondFunction()` then calls firstFunction()which is pushed into the stack.
3. `firstFunction()` returns and prints “Hello from firstFunction” to the console.
4. `firstFunction()` is pop off the stack.
5. The execution order then move to `secondFunction()`.
6. `secondFunction()` returns and print “The end from secondFunction” to the console.
7. `secondFunction()` is pop off the stack, clearing the memory.

A **stack overflow** occurs when there is a recursive function (function that calls itself) without an exit point.

### In Summary :

1. It is single-threaded. Meaning it can only do one thing at a time
2. Code execution is synchronous
3. A function invocation creates a stack frame that occupies a temporary memory
4. It works as a LIFO — Last In, First Out data structure

