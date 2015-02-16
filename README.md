# Guidelines - QuiNote Software Group
Notes on code, best practice, etc.


### Code Headers

Include a header at the top of each code file that anyone else might be expected to read. Headers should include the following information:

1. QuiNote Software Group 2015
2. Author[s]. If you edit a file, add your name to the authors.
3. A one-liner describing the file.
4. A brief description of input and output, if applicable. The general focus is on modular, object-oriented code with well-defined interfaces and extensive abstraction.
5. A TODO, if necessary/applicable, so that you're keeping documented track of issues and that other team members are aware of active problems in the code.

### Code Division

Separate HTML, CSS and JavaScript/jQuery into their own files. Separate code files by function to support modularity.

### Code Body Practices

Keep code files organized by function. For example, in a typical object-oriented JS file, there will be sections for global variables (try to avoid using these when possible, though--we have to be wary of overlapping variable names), prototype definitions and functions. These should be clearly marked as such:

```
//**************************************
// PROTOTYPE OBJECTS
//**************************************
```

This makes code files much easier to read. Also, consider marking important functions and prototypes, so that readers know where to look first. 

### Code Commenting

Include comments underneath the signature of each function and prototype definition that explains its purpose.

Include as many one-(or more) line comments as are necessary to explain the meaning of bits of code--this may double the length of a file, but makes it much easier to comprehend. Likewise, include newlines to space out distinct ideas with a function.

### Code Practices

1. Avoid writing excessively long lines. If a statement becomes too long to follow, consider breaking it up into logical constituents. 
2. Write as many helpers functions as you need. If you need a block of code that serves a general or oft called-for purpose, consider writing it out in a separate function. In particular, strive to abstract details from top-level functions (such as main access functions). 
