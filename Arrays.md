#What is an array?
An array is a collection of elements of the same type stored in contiguous memory.
ou access elements by index (starting from 0).

#Why use arrays?
Group related values together.
Easy traversal with loops.
Fast random access: reading arr[i] is O(1).

#Declaration & initialization
Syntax:
data_type array_name[size];
ex:
int arr[5];
size must be a positive integer.
Size must be known at compile time unless using VLA (Variable Length Array) in C99+:
Arrays cannot be resized once declared.

#different types of array declarations
1.int arr[5]; //Fixed-size array declaration
2.int arr[] = {10, 20, 30, 40}; //Declaration with initialization
3.int arr[5] = {1, 2, 3, 4, 5}; //Fixed-size with initialization
4.int arr[5] = {10, 20}; //Partial initialization (arr = {10, 20, 0, 0, 0})
5.char name[10] = "Hello"; //String (character array) declaration
6.char name[] = "Hello"; //without size 

#MULTI-DIMENSIONAL ARRAY
1.int matrix[3][3]; //2D array:
2.int matrix[2][3] = {
    {1, 2, 3},
    {4, 5, 6}
}; // with initialzation
3.int cube[2][3][4]; //3D array

#Array of pointers
1.int *arr[5];
2.int (*p)[5]; //Pointer to an array
3.int *arr = malloc(5 * sizeof(int)); //Dynamic array (using malloc)
4.const int arr[3] = {1, 2, 3};//Constant array
5.static int arr[5];//Static array
6.int arr[100];//Global array (Declared outside all functions.)













