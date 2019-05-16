[slide]
# While or For
***While*** and ***for*** loops both **repeat** a block of **code**

Use ***for*** when you know the **number of repetitions**

Use ***while*** when you don't know when you will meet the end condition

[/slide]

[slide]
# Problem: Odd Number
[code-task title="Odd Number" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads numbers from the console until it gets an **odd number**
* Prints the **odd** number
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2<br>4<br>8<br>3|3|
[/slide]

[slide]
# Solution: Odd Number
[code-task title="Odd Number" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
        int number = int.Parse(Console.ReadLine());
        while (number % 2 == 0)
        {
            number = int.Parse(Console.ReadLine());
        }
        Console.WriteLine(number);
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads numbers from the console until it gets an **odd number**
* Prints the **odd** number
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2<br>4<br>8<br>3|3|
[/slide]

[slide]
# Problem: Number Manipulator
[code-task title="Number Manipulator" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads a number from the console
* Reads the following commands:
* **Add** - Аdds 1 to the number
* **Subtract** - Subtracts 1 from the number
* **END** -  Prints the number and stops the program
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5<br>Add<br>End<br>|6|
|5<br>Subtract<br>End<br>|4|
[/slide]

[slide]
# Solution: Number Manipulator
[code-task title="Number Manipulator" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
        int number = int.Parse(Console.ReadLine());
        string command = Console.ReadLine();
        while (command != "END") {
        switch (command) {
            case "Add": number++; break;
            case "Subtract": number--; break;
        }
        command = Console.ReadLine();
        }
        Console.WriteLine(number);
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads a number from the console
* Reads the following commands:
* **Add** - Аdds 1 to the number
* **Subtract** - Subtracts 1 from the number
* **END** -  Prints the number and stops the program
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5<br>Add<br>End<br>|6|
|5<br>Subtract<br>End<br>|4|
[/slide]