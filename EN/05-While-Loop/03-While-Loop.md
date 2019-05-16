[slide]
# While Loop
Used to repeat a code block until an end condition is met

[image src="https://github.com/AlenPaunov/pb-interactive-course/blob/05-while-loop/assets/05-while-loop-2.png"/]
[/slide]

[slide]
# Problem: Decreasing Numbers
[code-task title="Decreasing Numbers" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
* Prints the numbers starting from the number to 1 (**inclusive**)
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|4|4<br>3<br>2<br>1|
[/slide]

[slide]
# Solution: Decreasing Numbers
[code-task title="Decreasing Numbers" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
        int number = int.Parse(Console.ReadLine());
        while (number >= 1)
        {
            Console.WriteLine(number);
            number--;
        }
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads a number from the console
* Prints the numbers starting from the number to 1 (**inclusive**)
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|4|4<br>3<br>2<br>1|
[/slide]

[slide]
# Problem: Numbers in Range
[code-task title="Numbers in Range" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads a **number** from the console
* Checks if the number is in the range between **1 and 100**
* If it isn't - it reads a **new one**
* If it is - **prints the number** and the program stops
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|-10<br>101<br>50|50|
[/slide]

[slide]
# Solution: Numbers in Range
[code-task title="Numbers in Range" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
        int num = int.Parse(Console.ReadLine());
        while (num < 1 || num > 100)
        {
            num = int.Parse(Console.ReadLine());
        }
        Console.WriteLine(num);
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads a **number** from the console
* Checks if the number is in the range between **1 and 100**
* If it isn't - it reads a **new one**
* If it is - **prints the number** and the program stops
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|-10<br>101<br>50|50|
[/slide]