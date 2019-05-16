[slide]
# Increment / Decrement Operators

Increment (++) operator increases the value by 1

Decrement (--) operator decreases the value by 1

Can be used pre and post fix

* Prefix: **++i**, **--i**
* Postfix: **i++**, **i--**

Both operators can be used only with numeric variables

[/slide]

[slide]
# Example:

Pre-decrement

```csharp
int a = 1; 
Console.WriteLine(--a); // 0: Decreases the value and then prints it
Console.WriteLine(a);   // 0
```
Post-decrement

```csharp
int a = 1; 
Console.WriteLine(a--); // 1: First prints the value and then decreases it
Console.WriteLine(a);   // 0
```
[/slide]

[slide]
# For Loop with Step

The step part in a for loop can either increase or decrease the value of a variable

```csharp
for (int i = 0; i < 10; i += 2)
  Console.WriteLine(i);
```
```csharp
// Always pay attention on the condition
for (int i = 10; i >= 0; i -= 2)
  Console.WriteLine(i);
```
[/slide]

[slide]
# Problem: Numbers Ending with 7
[code-task title="Numbers Ending with 7" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads a number n
* Prints all numbers from 7 to n, ending with 7
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|27|7<br>17<br>27|
|40|7<br>17<br>27<br>37|
[/slide]

[slide]
# Solution: Numbers Ending with 7
[code-task title="Numbers Ending with 7" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      int n = int.Parse(Console.ReadLine());
      for (int i = 7; i <= n; i += 10)
      {
        Console.WriteLine(i);
      }
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads a number n
* Prints all numbers from 7 to n, ending with 7
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|27|7<br>17<br>27|
|40|7<br>17<br>27<br>37|
[/slide]

[slide]
# Problem: Exam Countdown
[code-task title="Exam Countdown" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads an integer - count of days before an exam
* For each day prints: "{currentDay} days before the exam"
* At the end prints: "The exam has come"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|3 days before the exam<br>2 days before the exam<br>1 days before the exam<br>The exam has come|
[/slide]

[slide]
# Solution: Exam Countdown
[code-task title="Exam Countdown" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      int days = int.Parse(Console.ReadLine);
      for (int i = days; i >= 1; i -= 1)
      {
        Console.WriteLine($"{i} days before the exam");
      }
      Console.WriteLine("The exam has come");
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads an integer - count of days before an exam
* For each day prints: "{currentDay} days before the exam"
* At the end prints: "The exam has come"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|3 days before the exam<br>2 days before the exam<br>1 days before the exam<br>The exam has come|
[/slide]