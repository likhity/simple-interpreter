# C++ Interpreter

This C++ program interprets an input program and executes the instructions specified by that program.

The way in which this program interprets and executes is: it first creates an intermediate representation of the program (a linked list of instructions that the interpreter can easily understand and execute). It then executes the program by starting at the head of the linked list and executing each node one at a time.

Code in this language is written like this: 
- At the top of your program, you list the names of all of the variables that you will use.
- Then you write the body of your program containing all of your instructions. 
- At the bottom, you list all of the inputs to your program.

The instructions that it supports are:
1. Outputting (print) the value of a variable
2. Input a value from the inputs
3. Assigning a value to a variable (can be a single value or an expression that is to be evaluated by the interpreter)
4. `IF` statements
5. `FOR` statements
6. `WHILE` statements
7. `SWITCH` statements

An example program in this language is as follows:
```
a, b, c, d;
{
    input a;
    input b;
    FOR (c = b; c < 10; c = c + 1;)
    {
        d = 0;
        WHILE d < c
        {
            output d;
            d = d + 1;
        }
    }
}
1 2
```

This is the grammar of the language accepted by this interpreter:
![Language grammar](https://i.imgur.com/D9awdQf.png)

I cannot make the source code of this program public.