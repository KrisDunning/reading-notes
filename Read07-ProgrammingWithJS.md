[Return to Code 102 Notes Page](https://krisdunning.github.io/reading-notes/Code102Notes.html)

# Programming With JavaScript

*****

Code is run, or executed from the first line in the file down to the last line. Thats is the execution order, the flow. There are tools we can use to break that flow and move to specific predetermined locations in the code. Some of those tools are:

- Conditionals- `if`, `else`, `>`,`<`  these evaluate a condition and determine whether to move down the code flow or skip a section.

- Loops- Loops execute and re-execute a section of code until a condition is met or we `break` out of them.

- Functions- `functions ()` are named sections of code that can be called and sent variables. The code that is inside of a function is only executed when it is called by name. Otherwise it is skipped over in normal code flow.

The `function()` is a standard building block for developers to reduce the amount of code they write. It is often used to wrap a section of code that is repeatedly used. They are passed `arguments` when called, and inside the function definition the `arguments` are received by `parameters`.  For example:

~~~~
//defining the function//
    function functionName(parameter1Name,parameter2Name)
    {
        return parameter1Name+parameter2Name;
    }

//calling or "invoking" the function//
    functionNames(argument1,argument2);
~~~~

Functions can `return` a value but are not required to. In fact you can even use a `function()` as a variable. But more on that another time.  
Any variables declared inside a `function()` are considered to be locally scoped to the function. That means they only exist inside the `function()` curly braces ( `{ }` ).  

*****

[Return to Code 102 Notes Page](https://krisdunning.github.io/reading-notes/Code102Notes.html)