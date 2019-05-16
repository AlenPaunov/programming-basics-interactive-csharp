[slide]
# Problem: Building
[code-task title="Building" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Prints information about **apartments** (odd rows), **offices** (even rows) and the **last floor** (last row)
* Apartment ***"A\{buildingNum\}\{apartmentNum\}"***
* Office ***"O\{floorNum\}\{officeNum\}"***
* Floor ***"L\{buildingNum\}\{apartmentNum\}"***
* The numbers always start from **0**
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|6<br>4|L60 L61 L62 L63<br>A50 A51 A52 A53<br>O40 O41 O42 O43<br>A30 A31 A32 A33<br>O20 O21 O22 O23<br>A10 A11 A12 A13|
[/slide]

[slide]
# Solution: Building
[code-task title="Building" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
        int floors = int.Parse(Console.ReadLine());
        int rooms = int.Parse(Console.ReadLine());
        for (int i = floors; i >= 1; i--) 
        {
            for (int j = 0; j < rooms; j++) 
            {
                if (i == floors) // Print L{i}{j} Last Floor
                if (i % 2 == 0) // Print O{i}{j} Office
                if (i % 2 == 1) // Print A{i}{j} Apartment
            } 
            Console.WriteLine();
        }
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Prints information about **apartments** (odd rows), **offices** (even rows) and the **last floor** (last row)
* Apartment ***"A\{buildingNum\}\{apartmentNum\}"***
* Office ***"O\{floorNum\}\{officeNum\}"***
* Floor ***"L\{buildingNum\}\{apartmentNum\}"***
* The numbers always start from **0**
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|6<br>4|L60 L61 L62 L63<br>A50 A51 A52 A53<br>O40 O41 O42 O43<br>A30 A31 A32 A33<br>O20 O21 O22 O23<br>A10 A11 A12 A13|
[/slide]

[slide]
# Problem: Passwords
[code-task title="Passwords" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Generates custom **3 digit** passwords, which meet the following conditions:
* The **first** digit is an **even** number
* The **second** digit is an **odd** number
* The **third** is the **product** of the first two
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|6|212 236 2510 414 4312 4520 616 6318 6530|
|5|212 236 2510 414 4312 4520|
[/slide]

[slide]
# Solution: Passwords
[code-task title="Passwords" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
        int n = int.Parse(Console.ReadLine());
        for (int i = 1; i <= n; i++)
        {
            for (int j = 1; j <= n; j++)
            {
                if (i % 2 == 0 && j % 2 != 0)
                {
                    Console.Write($"{i}{j}{i * j} ");
                }
            }
        }
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Generates custom **3 digit** passwords, which meet the following conditions:
* The **first** digit is an **even** number
* The **second** digit is an **odd** number
* The **third** is the **product** of the first two
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|6|212 236 2510 414 4312 4520 616 6318 6530|
|5|212 236 2510 414 4312 4520|
[/slide]

[slide]
# Problem: Magic Number
[code-task title="Magic Number" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads a **number - n**, from the console
* Finds all **3-digit numbers**:
* Forming **n** as a product of the multiplication of their digits
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|113<br>131<br>311|
|1|111|
[/slide]

[slide]
# Solution: Magic Number
[code-task title="Magic Number" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
        int magicNumber = int.Parse(Console.ReadLine());
        for (int i = 1; i <= 9; i++)
        {
            for (int j = 1; j <= 9; j++)
            { 
                for (int k = 1; k <= 9; k++)
                {
                    if (i * j * k == magicNumber)
                    // TODO: Print {i}{j}{k}
                }
            }
        }
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads a **number - n**, from the console
* Finds all **3-digit numbers**:
* Forming **n** as a product of the multiplication of their digits
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|113<br>131<br>311|
|1|111|
[/slide]

[slide]
# Problem: Travelling
[code-task title="Travelling" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads a **destination** and **needed budget** for destination
* Continues reading numbers - amounts of money, until they are **enough** for the destination
* If it receives the command **"End"** the program ends
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|Philippines<br>1000<br>550<br>450|Going to Philippines!|
[/slide]

[slide]
# Solution: Travelling
[code-task title="Travelling" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
        string townName = string.Empty;
        double currentMoney = 0;
        while ((townName = Console.ReadLine()) != "End") 
        {
            double neededMoney = double.Parse(Console.ReadLine());
            while (currentMoney < neededMoney) 
            {
                double money = double.Parse(Console.ReadLine());
                currentMoney += money;
            }
            Console.WriteLine($"Going to {townName}!");
            currentMoney = 0;
        }
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads a **destination** and **needed budget** for destination
* Continues reading numbers - amounts of money, until they are **enough** for the destination
* If it receives the command **"End"** the program ends
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|Philippines<br>1000<br>550<br>450|Going to Philippines!|
[/slide]

[slide]
# Problem: Prime Numbers
[code-task title="Prime Numbers" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads two numbers from the console
* Prints the prime number in that range
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1<br>50|1 2 3 5 7 11 13 17 19 23 29 31 37 41 43 47|
[/slide]

[slide]
# Solution: Prime Numbers
[code-task title="Prime Numbers" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
        int n = int.Parse(Console.ReadLine());
        int m = int.Parse(Console.ReadLine());
        for (int num = n; num <= m; num++) 
        {
            bool prime = true;
            int divider = 2;
            int maxDivider = (int)Math.Sqrt(num);
            while (divider <= maxDivider) 
            {
                if (num % divider == 0) 
                {
                    prime = false;
                    break;
                }
                divider++;
            }
            if (prime) Console.WriteLine(num);
        }
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads two numbers from the console
* Prints the prime number in that range
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1<br>50|1 2 3 5 7 11 13 17 19 23 29 31 37 41 43 47|
[/slide]

[slide]
# Problem: Unique PIN Codes
[code-task title="Unique PIN Codes" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads 3 digits - each of them is an upper limit
* Generates unique 3 digit PIN Codes, which meet the following conditions:
* They are in the range
* The first and the third digit must be even
* The second digit must be a prime  number in the range \[2…7\]
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3<br>5<br>5|222<br>224<br>232<br>234<br>252<br>254|
[/slide]

[slide]
# Solution: Unique PIN Codes
[code-task title="Unique PIN Codes" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
        int n1 = int.Parse(Console.ReadLine());
        int n2 = int.Parse(Console.ReadLine());
        int n3 = int.Parse(Console.ReadLine());
        for (int first = 1; first <= n1; first++) 
        {
            for (int second = 1; second <= n2; second++)
            {
                for (int third = 1; third <= n3; third++) 
                {  
                    if (first % 2 == 0 && third % 2 == 0)
                    // TODO: Checks if the second value is 2, 3, 5 or 7 
            and prints the 3 digits one after another
                }
            }
        }
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads 3 digits - each of them is an upper limit
* Generates unique 3 digit PIN Codes, which meet the following conditions:
* They are in the range
* The first and the third digit must be even
* The second digit must be a prime  number in the range \[2…7\]
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3<br>5<br>5|222<br>224<br>232<br>234<br>252<br>254|
[/slide]

[slide]
# Problem: Letter Combinations
[code-task title="Letter Combinations" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Prints letters combinations and the count of the printed combinations
* You will receive the range of letters on the first and second line
* On the third line, you will receive a letter, which you must ignore - don't print combinations with it
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|a<br>b<br>c|aaa aac aca acc caa cac cca ccc|
[/slide]

[slide]
# Solution: Letter Combinations
[code-task title="Letter Combinations" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
        char startLetter = char.Parse(Console.ReadLine());
        char endLetter = char.Parse(Console.ReadLine());
        char avoidLetter = char.Parse(Console.ReadLine());
        int counter = 0;
        for (char first = startLetter; first <= endLetter; first++)
        {
            for (char second = startLetter; second <= endLetter; second++)
            {
                for (char third = startLetter; third <= endLetter; third++)
                {
                    if (first != avoidLetter && second != avoidLetter && third != avoidLetter)
                    {
                        // TODO: Print the combinations
                    }
                    // TODO: Print the counter
                }
            }
        }
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Prints letters combinations and the count of the printed combinations
* You will receive the range of letters on the first and second line
* On the third line, you will receive a letter, which you must ignore - don't print combinations with it
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|a<br>b<br>c|aaa aac aca acc caa cac cca ccc|
[/slide]

[slide]
# Problem: Happy Numbers
[code-task title="Happy Numbers" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
* Prints all 4 digit numbers, which meet the following conditions:
* When you split them in two pairs and add the first digit to the second - the result equals n
* When you add the first two digits to each other, the result must be divisible by n without a remainder
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|1212 1221 2112 2121|
[/slide]

[slide]
# Solution: Happy Numbers
[code-task title="Happy Numbers" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
        int number = int.Parse(Console.ReadLine());
        for (int firstDigit = 1; firstDigit <= 9; firstDigit++)
        {
            for (int secDigit = 1; secDigit <= 9; secDigit++)
            {
                for (int thirdDigit = 1; thirdDigit <= 9; thirdDigit++)
                {
                    for (int forthDigit = 1; forthDigit <= 9; forthDigit++)
                    {
                        if (firstDigit + secDigit == thirdDigit + forthDigit)
                        {
                            if (number % (firstDigit + secDigit) == 0)
                            // TODO: Print the number        
                        }
                    }
                }
            }
        }
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads a number n
* Prints all 4 digit numbers, which meet the following conditions:
* When you split them in two pairs and add the first digit to the second - the result equals n
* When you add the first two digits to each other, the result must be divisible by n without a remainder
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|1212 1221 2112 2121|
[/slide]
