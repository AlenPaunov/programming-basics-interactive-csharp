[slide]
# Problem: Sum Digits
[code-task title="Sum Digits" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
* **Sums** the **digits** of a number
* Prints the sum
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5634|18|
[/slide]

[slide]
# Solution: Sum Digits
[code-task title="Sum Digits" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      int n = int.Parse(Console.ReadLine());
      int sum = 0;
      while (n > 0)
      {
        sum += n % 10;
        n /= 10;
      }
      Console.WriteLine(sum);
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads a number from the console
* **Sums** the **digits** of a number
* Prints the sum
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5634|18|
[/slide]

[slide]
# Problem: Favorite Book
[code-task title="Favorite Book" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads a **book's name** from the console
* Receives names until it gets the **same book**
* Prints **"Book found!"** and stops afterwards
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|Alice in Wonderland<br>Winnie the Pooh<br>Peter Pan<br>Alice in Wonderland|Book Found!|
[/slide]

[slide]
# Solution: Favorite Book
[code-task title="Favorite Book" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      string favoriteBook = Console.ReadLine();
      string book = Console.ReadLine();
      while(book != favoriteBook)
      {
        book = Console.ReadLine();
      }
      Console.WriteLine("Book found!");
    }
}
```
[/code-editor]
[task-description]
Write a program, which: 

* Reads a **book's name** from the console
* Receives names until it gets the **same book**
* Prints **"Book found!"** and stops afterwards
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|Alice in Wonderland<br>Winnie the Pooh<br>Peter Pan<br>Alice in Wonderland|Book Found!|
[/slide]

[slide]
# Problem: Min and Max
[code-task title="Min and Max" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Receives integers until **"END"**
* Prints the **biggest** and the **smallest** integer
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|10<br>20<br>304<br>0<br>50<br>END|Max number: 304<br>Min number: 0|
[/slide]

[slide]
# Solution: Min and Max
[code-task title="Min and Max" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      string line = Console.ReadLine();
      int min = int.MaxValue;
      int max = int.MinValue;
      while (line != "END") {
        int n = int.Parse(line);
        if (n < min)
          min = n;
        if (n > max)
          max = n;
        line = Console.ReadLine();
      } 
      // TODO: Print output
    }
}
```
[/code-editor]
[task-description]
Write a program, which: 

* Receives integers until **"END"**
* Prints the **biggest** and the **smallest** integer
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|10<br>20<br>304<br>0<br>50<br>END|Max number: 304<br>Min number: 0|
[/slide]

[slide]
# Problem: Special Number
[code-task title="Special Number" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Receives integer
* Prints "\{num\} is special" if the number is special
* Special number is number divisible by all of its digits without remainder
* Otherwise, prints "\{num\} is not special"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|23|23 is not special|
|44|44 is special|
[/slide]

[slide]
# Solution: Special Number
[code-task title="Special Number" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      int originNumber = int.Parse(Console.ReadLine());
      int number = originNumber;
      bool isSpecial = true;
      while (number > 0) {
        int digit = number % 10;
        number /= 10;
        if (originNumber % digit != 0) {
          isSpecial = false;
          break;
        }
      }
      //TODO: Print the final message
    }
}
```
[/code-editor]
[task-description]
Write a program, which: 

* Receives integer
* Prints "\{num\} is special" if the number is special
* Special number is number divisible by all of its digits without remainder
* Otherwise, prints "\{num\} is not special"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|23|23 is not special|
|44|44 is special|
[/slide]

[slide]
# Problem: Special Bonus
[code-task title="Special Bonus" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads a special integer number from the console
* Keeps reading integers until it finds the same one
* When it finds it, it increases the value of the **previous** number **before it** with 20% and prints it
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|25<br>20<br>30<br>25|36|
[/slide]

[slide]
# Solution: Special Bonus
[code-task title="Special Bonus" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      int special = int.Parse(Console.ReadLine());
      int number = Console.ReadLine();
      int previous = number;
      while(true) {
        if(number == special) {
          previous += previous * 0.2;
          break;
        }
        previous = number
        number = Console.ReadLine();
      }
      Console.WriteLine(previous);
    }
}
```
[/code-editor]
[task-description]
Write a program, which: 

* Reads a special integer number from the console
* Keeps reading integers until it finds the same one
* When it finds it, it increases the value of the **previous** number **before it** with 20% and prints it
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|25<br>20<br>30<br>25|36|
[/slide]

[slide]
# Problem: Sequence 2k + 1
[code-task title="Sequence 2k + 1" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads a number **n** from the console
* Prints a **sequence** of numbers, which are **<= n** and satisfy the following condition:
* Each number is equal to the previous one multiplied by **2** plus **1**
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|8|1<br>3<br>7|
[/slide]

[slide]
# Solution: Sequence 2k + 1
[code-task title="Sequence 2k + 1" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      int n = int.Parse(Console.ReadLine());
      int k = 1;
      while(k <= n)
      {
        Console.WriteLine(k);
        k = k * 2 + 1;
      }
    }
}
```
[/code-editor]
[task-description]
Write a program, which: 

* Reads a number **n** from the console
* Prints a **sequence** of numbers, which are **<= n** and satisfy the following condition:
* Each number is equal to the previous one multiplied by **2** plus **1**
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|8|1<br>3<br>7|
[/slide]

[slide]
# Problem: Account Balance
[code-task title="Account Balance" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Receives an integer **n** - count of transactions
* Receives the amount of money for each transaction
* Adds the money to the balance and prints: "***Increase***: \{money\} " and calculates and prints the total balance
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3<br>5.51<br>69.42<br>100|Increase: 5.51<br>Increase: 69.42<br>Increase: 100<br>Total: 174.93|
[/slide]

[slide]
# Solution: Account Balance
[code-task title="Account Balance" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      int n = int.Parse(Console.ReadLine());
      double balance = 0.0;
      while(n != 0) {
        double amount = double.Parse(Console.ReadLine());
        balance += amount;
        Console.WriteLine($"Increase: {amount:f2}");
        n--;
      }
      Console.WriteLine($"Total: {balance:f2}");
    }
}
```
[/code-editor]
[task-description]
Write a program, which: 

* Receives an integer **n** - count of transactions
* Receives the amount of money for each transaction
* Adds the money to the balance and prints: "***Increase***: \{money\} " and calculates and prints the total balance
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3<br>5.51<br>69.42<br>100|Increase: 5.51<br>Increase: 69.42<br>Increase: 100<br>Total: 174.93|
[/slide]