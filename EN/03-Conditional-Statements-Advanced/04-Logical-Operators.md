[slide]
# Logical Operators
Used to perform logical operations

The logical operators are:

  * AND (**&&**)
  * OR (**||**)
  * Logical negation (**!**)

Brackets **()** change the order

Explanation

[image src="https://github.com/AlenPaunov/pb-interactive-course/blob/03-conditional-statements-advanced/assets/03-conditional-statements-advanced-1.png"/]
[/slide]

[slide]
# Logical AND (&&)
Returns the boolean value true if operands are true and returns false otherwise

```csharp
if (x >= x1 && x <= x2 && y >= y1 && y <= y2)
```
[/slide]
[slide]
# Problem: Bonus Points
[code-task title="Bonus Points" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program that applies bonus to given points

  * If points are between 0 and 3, adds 5
  * If points are between 4 and 6, adds 15
  * If points are between 7 and 9, adds 20
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|4|19|
[/slide]

[slide]
# Solution: Bonus Points
[code-task title="Bonus Points" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      int points = int.Parse(Console.ReadLine());
      if (points >= 0 && points <= 3)
        points += 5;
      else if (points >= 4 && points <= 6)
        points += 15;
      else if (points >= 7 && points <= 9)
        points += 20;

      Console.WriteLine(points);
    }
}
```
[/code-editor]
[task-description]
Write a program that applies bonus to given points

  * If points are between 0 and 3, adds 5
  * If points are between 4 and 6, adds 15
  * If points are between 7 and 9, adds 20
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|4|19|
[/slide]

[slide]
# Logical OR (||)
The result of the expression is ***true*** if one of the operands is ***true***, otherwise the result is ***false***

```csharp
s == "tea" || s == "water" || s == "spaghetti"
```
[/slide]

[slide]
# Problem: Food or Drink
[code-task title="Food or Drink" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

  * Reads single line and print "***drink***", "***food***" or "***unknown***"
  * Foods: curry, noodles, sushi, spaghetti 
  * Drinks: tea, water, coffee
  * Everything else is unknown
[/task-description]
[code-io /]
[/code-task]
[/slide]

[slide]
# Solution: Food or Drink
[code-task title="Food or Drink" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      string s = Console.ReadLine();
      if (s == "curry" || s == "noodles" || 
          s == "sushi" || s == "spaghetti")
        Console.WriteLine("food");
      else if (s == "tea" || s == "water" || s == "coffee")
        Console.WriteLine("drink");
      else
        Console.WriteLine("unknown");
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

  * Reads single line and print "***drink***", "***food***" or "***unknown***"
  * Foods: curry, noodles, sushi, spaghetti 
  * Drinks: tea, water, coffee
  * Everything else is unknown
[/task-description]
[code-io /]
[/code-task]
[/slide]

[slide]
# Logical NOT (!)
Returns ***true***, if the operand is ***false***, and ***false***, if the operand is ***true***

Example:

  * Number is valid if is in the range [100…200] or is equal to 0
```csharp
bool inRange = (num >= 100 && num <= 200) || 
              num == 0;
if (!inRange)
  Console.WriteLine("invalid");
```
[/slide]