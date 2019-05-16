[slide]
# Series of Conditions
The ***if-else*** statement can be in series

```csharp
if (…) 
  // code
else if (…) 
  // code
else if (…) 
  // code
// If one condition is true, the program will NOT check the rest of the conditions
```

Example

The program checks the first condition, finds that it is *true* and ends

```csharp
int a = 7;
if (a > 4) 
  Console.WriteLine("Bigger than 4"); 
else if (a > 5)
  Console.WriteLine("Bigger than 5"); 
else 
  Console.WriteLine("Smaller or equal to 4"); 
// The output is only "Bigger than 4"
```
[/slide]

[slide]
# Problem: Number 1...9
[code-task title="Number 1...9" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program, which prints a number as text: 

  * Read an **integer** in the range [1…100]
  * Print its value in the form of text (in English)
  * If the number is **greater** than 9 print ***"Number too big"***
[/task-description]
[code-io /]
[/code-task]

# Sample Input and Output
|Input|Output|
|-----|------|
|7|seven|
|10|Number too big|
|2|two|
[/slide]

[slide]
# Solution: Number 1...9
[code-task title="Number 1...9" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      int num = int.Parse(Console.ReadLine());
      if (num == 1)
        Console.WriteLine("one");
      else if (num == 2)
        Console.WriteLine("two");
      // TODO: Add the rest of the conditions 
      // …
      else
      Console.WriteLine("Number too big");
    }
}
```
[/code-editor]
[task-description]
Write a program, which prints a number as text:

  * Read an **integer** in the range [1…100]
  * Print its value in the form of text (in English)
  * If the number is **greater** than 9 print ***"Number too big"***
[/task-description]
[code-io /]
[/code-task]

# Sample Input and Output
|Input|Output|
|-----|------|
|7|seven|
|10|Number too big|
|2|two|
[/slide]