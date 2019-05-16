[slide]
# Variables
In programming **data** is stored in **variables**

  * Variables store data in a piece of the memory
  * Variable read: retrieve the stored data
  * Variable write: modify the stored information
  
Declaring, initializing, reading and changing a variable in C#:

```csharp
int age = 5;
```
```csharp
age = age + 1;
```
```csharp
Console.WriteLine(age);
```
[/slide]

[slide]
# Data Types in C#
Integer number – **int** (e.g. 5, 0, 120, -250)

Floating-point number – **double** (e.g. 3.14159, 0.5)

Boolean (true / false) – **bool** (true or false)

Unicode characters (letters) – **char** (e.g. 'X', '#', '\n')

Unicode strings (text) – **string** (e.g. "Hello C#")

Date and time – **DateTime** (e.g. 6-Jun-2020 9:18:34)

[/slide]

[slide]
# Expressions and Statements
**Expressions** == **variables** and **values**, combined with **operators**

```csharp
a = b * 2;
// 2 is a literal value expression
// a = b * 2 is an assignment expression
// b is a variable expression
// b * 2 is an arithmetic expression
```

Statements - Commands / actions to be executed

```csharp
a = b * 2;
// Get the current value stored in b
// Multiply that value by 2
// Store the result back into another variable we call a
```
[/slide]