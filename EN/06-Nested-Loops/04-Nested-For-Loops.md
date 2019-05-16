[slide]
# Nested for Loops
Statements that consist of several **loops** located **inside each other**

**Nested loops** are used:

* To execute an **action**, which **executes** multiple **actions**
* To make more **complex** calculations and variations

```csharp
for (int i = 1; i <= n; i+=3) 
{
   for (int j = 1; j <= n; j+=3)
   {
      for (int k = 1; k <= n; k+=3)
      {
        // ...
      }
   }
}
```
[/slide]

[slide]
# Nested for Loops
The syntax for a **nested ***for*** loop in C#** is as follows

```csharp
for (init; condition; increment) 
{   // Outer Loop 
  for (init; condition; increment) 
  { // Inner Loop
     Statement
  }
}
```
```csharp
int a = 3;
int b = 3;
for (int i = 0; i < a; i++) 
{
  Console.WriteLine("i = " + i);
  for (int j = 0; j < b; j++) 
    // Print "j = " and value of j
}
```
[/slide]

[slide]
# Problem: Triangle of Stars
[code-task title="Triangle of Stars" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      // Write code here
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads the **height** of a triangle from the console
* Prints a **triangle of stars**
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|\*<br>\*\*<br>\*\*\*<br>\*\*\*\*<br>\*\*\*\*\*|
[/slide]

[slide]
# Solution: Triangle of Stars
[code-task title="Triangle of Stars" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
        int height = int.Parse(Console.ReadLine());
        for (int i = 1; i <= height;  i++)
        {
            for (int j = 1; j <= i; j++)
            {
                Console.Write("*");
            }
            Console.WriteLine();
        }
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads the **height** of a triangle from the console
* Prints a **triangle of stars**
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|\*<br>\*\*<br>\*\*\*<br>\*\*\*\*<br>\*\*\*\*\*|
[/slide]