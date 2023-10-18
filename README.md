# Pointer-operations

THEORY 

Pointers are symbolic representations of addresses. They enable programs to simulate call-by-reference as well as to create and manipulate dynamic data structures. Iterating over elements in arrays or other data structures is one of the main use of pointers. 

The address of the variable you’re working with is assigned to the pointer variable that points to the same data type (such as an int or string).

Syntax:

datatype *var_name; 
int *ptr;   // ptr can point to an address which holds int data

How to use a pointer?
Define a pointer variable
Assigning the address of a variable to a pointer using the unary operator (&) which returns the address of that variable.
Accessing the value stored in the address using unary operator (*) which returns the value of the variable located at the address specified by its operand.
The reason we associate data type with a pointer is that it knows how many bytes the data is stored in. When we increment a pointer, we increase the pointer by the size of the data type to which it points.

References and Pointers
There are 3 ways to pass C++ arguments to a function:

Call-By-Value

Call-By-Reference with a Pointer Argument

Call-By-Reference with a Reference Argument

ALGORITHM

Call by Value

1.Define a function that takes a pointer as a parameter.

2.Inside the function, you can access and modify the data pointed to by ptr. Changes made to *ptr will affect the original data in the calling code.

3.In the main program, declare a variable and initialize it.

Call by Reference

1.Define a function that takes a pointer as a parameter.

2.Inside the function, you can access and modify the value at the memory location pointed to by x. Changes made to *x will affect the original variable from the calling code.

3.Call the function from your main program and pass the address (pointer) of the variable you want to modify.

These algorithms demonstrate how to implement call by value and call by reference using pointers in C++. Remember that in the call by value method, a copy of the argument is passed to the function, while in the call by reference method using pointers, the function receives the address of the original variable, allowing it to modify the original variable.

EXPECTED OUTPUT

Value of x is:500

Value of y is:100

