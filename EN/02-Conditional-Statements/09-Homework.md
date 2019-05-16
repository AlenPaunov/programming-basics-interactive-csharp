[slide]
# Problem: Guess the Password
[code-task title="Guess the Password" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program to check a password:

  * Read a string: the password guess
  * Print "Welcome" if the password guess is "s3cr3t!"
  * Print "Wrong password!" in all other cases 
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|s3cr3t!|Welcome|
|qwerty|Wrong password!|
[/slide]

[slide]
# Solution: Guess the Password
[code-task title="Guess the Password" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      string password = Console.ReadLine();
      if (password == "s3cr3t!") {
        Console.WriteLine("Welcome");
      }
      else {
        Console.WriteLine("Wrong password!");
      }
    }
}
```
[/code-editor]
[task-description]
Write a program to check a password:

  * Read a string: the password guess
  * Print "Welcome" if the password guess is "s3cr3t!"
  * Print "Wrong password!" in all other cases 
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|s3cr3t!|Welcome|
|qwerty|Wrong password!|
[/slide]

[slide]
# Problem: Boiling Water
[code-task title="Boiling Water" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program, which checks for hot water: 

  * Read a floating-point number: the water temperature (in °C)
  * Print "The water is boiling" if the number > 100
  * Prints "The water is not hot enough" in all other cases 
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|104.8|The water is boiling|
|29|The water is not hot enough|
[/slide]

[slide]
# Solution: Boiling Water
[code-task title="Boiling Water" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      double temperature = double.Parse(Console.ReadLine());
      if (temperature > 100)
        Console.WriteLine("The water is boiling"); 
      else
        Console.WriteLine("The water is not hot enough");
    }
}
```
[/code-editor]
[task-description]
Write a program, which checks for hot water: 

  * Read a floating-point number: the water temperature (in °C)
  * Print "The water is boiling" if the number > 100
  * Prints "The water is not hot enough" in all other cases 
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|104.8|The water is boiling|
|29|The water is not hot enough|
[/slide]

[slide]
# Problem: Speed Info
[code-task title="Speed Info" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program to check for fast / slow speed: 

  * Read the speed (a floating-point number)
  * Print "Slow" if the speed <= 30
  * Print "Fast" if the speed > 30
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|30|Slow|
|60|Fast|
[/slide]

[slide]
# Solution: Speed Info
[code-task title="Speed Info" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      double speed = double.Parse(
      Console.ReadLine());
      if (speed <= 30)
      {
        Console.WriteLine("Slow");
      }
      else
      {
        Console.WriteLine("Fast");
      }
    }
}
```
[/code-editor]
[task-description]
Write a program to check for fast / slow speed: 

  * Read the speed (a floating-point number)
  * Print "Slow" if the speed <= 30
  * Print "Fast" if the speed > 30
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|30|Slow|
|60|Fast|
[/slide]

[slide]
# Problem: Area of Figures
[code-task title="Area of Figures" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program to calculate the area of different figures:

  * Read a string: the figure type
  * Read a number (the size) or two numbers for rectangle (sizes)
  * Checks if the entered figure is square, rectangle or circle
  * Print the calculated area formatted to the second decimal
  * For unknown figure print "Unknown figure"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|square<br>5|25.00|
[/slide]

[slide]
# Solution: Area of Figures
[code-task title="Area of Figures" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      string figure = Console.ReadLine();
      double area = 0;
      if (figure == "square")
        // Read the side and calculate the area
      else if (figure == "rectangle")
        // Read width, height and calculate the area
      else if (figure == "circle")
        // Read the radius and calculate the area
      else // Print "Unknown figure"
      Console.WriteLine("{0:0.00}", area);
    }
}
```
[/code-editor]
[task-description]
Write a program to calculate the area of different figures: 

  * Read a string: the figure type
  * Read a number (the size) or two numbers for rectangle (sizes)
  * Checks if the entered figure is square, rectangle or circle
  * Print the calculated area formatted to the second decimal
  * For unknown figure print "Unknown figure"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|square<br>5|25.00|
[/slide]

[slide]
# Problem: Tickets
[code-task title="Tickets" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program to calculate a ticket price:

  * Read a ticket type: either student or regular
  * Print the price in the following format "${price}":
  * Student ticket price: 1.00
  * Regular ticket price: 1.60
  * For invalid type print "Invalid ticket type!"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|student|$1.00|
|regular|$1.60|
[/slide]

[slide]
# Solution: Tickets
[code-task title="Tickets" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      string ticketType = Console.ReadLine();
      if (ticketType == "student")
        Console.WriteLine("$1.00");
      else if (ticketType == "regular")
        Console.WriteLine("$1.60");
      else
        Console.WriteLine("Invalid ticket type!");
    }
}
```
[/code-editor]
[task-description]
Write a program to calculate a ticket price:

  * Read a ticket type: either student or regular
  * Print the price in the following format "${price}":
  * Student ticket price: 1.00
  * Regular ticket price: 1.60
  * For invalid type print "Invalid ticket type!"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|student|$1.00|
|regular|$1.60|
[/slide]

[slide]
# Problem: Coffee Shop
[code-task title="Coffee Shop" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program to calculate the drink price in a coffee shop:

  * Read a drink: either "coffee" or "tea"
  * Read an extra: either "sugar" or "no"
  * Print the price in format "Final price: ${price}"
Prices:

  * Coffee price: 1.00
  * Tea price: 0.60
  * Sugar price: 0.40
[/task-description]
[code-io /]
[/code-task]
[/slide]

[slide]
# Solution: Coffee Shop
[code-task title="Coffee Shop" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      string drink = Console.ReadLine();
      string extra = Console.ReadLine();
      double price = 0;
      if (drink == "coffee")
        // Set the price to 1.00
      else if (drink == "tea")
        // Set the price to 0.60
      if (extra == "sugar")
        // Increase the price by 0.40
      Console.WriteLine($"Final price: ${price}");
    }
}
```
[/code-editor]
[task-description]
Write a program to calculate the drink price in a coffee shop:

  * Read a drink: either "coffee" or "tea"
  * Read an extra: either "sugar" or "no"
  * Print the price in format "Final price: ${price}"
Prices:

  * Coffee price: 1.00
  * Tea price: 0.60
  * Sugar price: 0.40
[/task-description]
[code-io /]
[/code-task]
[/slide]

[slide]
# Problem: Valid Triangle
[code-task title="Valid Triangle" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program to check if a triangle is valid by its sizes:

  * Read 3 integers: the sides of a triangle
  * Checks if each side is lesser than the sum of the other 2
  * Prints "Valid Triangle" if the above condition is met
  * Prints "Invalid Triangle" otherwise 
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3<br>4<br>5|Valid Triangle|
[/slide]

[slide]
# Solution: Valid Triangle
[code-task title="Valid Triangle" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      int a = int.Parse(Console.ReadLine());
      int b = int.Parse(Console.ReadLine());
      int c = int.Parse(Console.ReadLine());
      bool isValidTriangle = true;
      if (a + b <= c)
        // Set isValidTriangle to false
      else if (a + c <= b)
        // Set isValidTriangle to false
      else if (b + c <= a)
        // Set isValidTriangle to false
      // Finally: print the result on the console
    }
}
```
[/code-editor]
[task-description]
Write a program to check if a triangle is valid by its sizes:

  * Read 3 integers: the sides of a triangle
  * Checks if each side is lesser than the sum of the other 2
  * Prints "Valid Triangle" if the above condition is met
  * Prints "Invalid Triangle" otherwise 
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3<br>4<br>5|Valid Triangle|
[/slide]