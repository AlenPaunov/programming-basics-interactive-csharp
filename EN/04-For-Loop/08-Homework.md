[slide]
# Problem: Number Sequence
[code-task title="Number Sequence" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads n representing the count of numbers to read next
* Finds the max and the min numbers
* Prints them on the console
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5<br>10<br>20<br>304<br>0<br>50|Max number: 304<br>Min number: 0|
[/slide]

[slide]
# Solution: Number Sequence
[code-task title="Number Sequence" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
        int n = int.Parse(Console.ReadLine());
        int min = int.MaxValue;
        int max = int.MinValue;
        for (int i = 0; i < n; i++)
        {
            int num = int.Parse(Console.ReadLine());
            if (num < min) min = num;
            if (num > max) max = num;
        }
        Console.WriteLine($"Max number: {max}");
        Console.WriteLine($"Min number: {min}");
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads n representing the count of numbers to read next
* Finds the max and the min numbers
* Prints them on the console
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5<br>10<br>20<br>304<br>0<br>50|Max number: 304<br>Min number: 0|
[/slide]

[slide]
# Problem: Power Of Numbers
[code-task title="Power Of Numbers" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads p – the power and n – the number
* Prints the result of n powered by p
* Don't use Math.Pow()
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5<br>2|32|
|4<br>3|81|
[/slide]

[slide]
# Solution: Power Of Numbers
[code-task title="Power Of Numbers" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
        int p = int.Parse(Console.ReadLine());
        int n = int.Parse(Console.ReadLine());
        int result = 1;
        for(int i = 0; i < p; i++)
        {
          result = result * n;
        }
        Console.WriteLine(result);
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads p – the power and n – the number
* Prints the result of n powered by p
* Don't use Math.Pow()
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5<br>2|32|
|4<br>3|81|
[/slide]

[slide]
# Problem: Equal Pairs
[code-task title="Equal Pairs" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads number n and n pairs of numbers
* Prints "Yes, value={sum}", if the sum of all pairs is the same
* Otherwise, prints "No, maxdiff={diff}"
* diff is the max difference in the sum between two pairs
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2<br>-1<br>0<br>0<br>-1|Yes, value=-1|
[/slide]

[slide]
# Solution: Equal Pairs
[code-task title="Equal Pairs" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
        int n = int.Parse(Console.ReadLine());
        int prevSum = 0;
        int maxDiff = 0;
        bool areEqual = true;
        for (int i = 0; i < n; i++) {
        int a = int.Parse(Console.ReadLine());
        int b = int.Parse(Console.ReadLine());
        if (i > 0) {
            if (maxDiff < Math.Abs(prevSum - a - b))
            maxDiff = Math.Abs(prevSum - a - b);
            if (areEqual && a + b != prevSum) 
            areEqual = false;
        }
        prevSum = a + b;
        }
        // TODO: Print the result
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads number n and n pairs of numbers
* Prints "Yes, value={sum}", if the sum of all pairs is the same
* Otherwise, prints "No, maxdiff={diff}"
* diff is the max difference in the sum between two pairs
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2<br>-1<br>0<br>0<br>-1|Yes, value=-1|
[/slide]

[slide]
# Problem: Bigger Number
[code-task title="Bigger Number" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads n - number representing amount of input numbers
* Reads n numbers
* Finds and prints the biggest number
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3<br>40<br>90<br>50<br>|90|
|-3<br>-40<br>-90<br>-50<br>|-40|
[/slide]

[slide]
# Solution: Bigger Number
[code-task title="Bigger Number" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
        int n = int.Parse(Console.ReadLine());
        int maxNumber = int.MinValue;
        for (int i = 1; i <= n; i++) {
        int number = int.Parse(Console.ReadLine());
        if (number > maxNumber) {
            maxNumber = number;
        }
        }
        Console.WriteLine(maxNumber);
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads n - number representing amount of input numbers
* Reads n numbers
* Finds and prints the biggest number
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3<br>40<br>90<br>50<br>|90|
|-3<br>-40<br>-90<br>-50<br>|-40|
[/slide]

[slide]
# Problem: Zig Zag Sum
[code-task title="Zig Zag Sum" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads n - number representing amount of input numbers
* Reads n numbers 
* For every even line adds the number to the result
* For every odd line subtracts the number from the result
* Prints the result
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2<br>10<br>20|-30|
[/slide]

[slide]
# Solution: Zig Zag Sum
[code-task title="Zig Zag Sum" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
        int n = int.Parse(Console.ReadLine());
        int sum = 0;
        for (int i = 1; i <= n; i++) {
        int m = int.Parse(Console.ReadLine());
        if (i % 2 == 0) sum += m;
        else sum -= m;
        }
        Console.WriteLine(sum);
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads n - number representing amount of input numbers
* Reads n numbers 
* For every even line adds the number to the result
* For every odd line subtracts the number from the result
* Prints the result
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2<br>10<br>20|-30|
[/slide]

[slide]
# Problem: Divide Without Remainder
[code-task title="Divide Without Remainder" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads n and n numbers
* Finds in percentage how many of them can divide without remainder at 2, 3 and 4
* Prints percentages p1, p2 and p3, formatted to the second digit
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3<br>3<br>6<br>9|33.33%<br>100.00%<br>0.00%|
|3<br>4<br>6<br>3|66.67%<br>66.67%<br>33.33%|
[/slide]

[slide]
# Solution: Divide Without Remainder
[code-task title="Divide Without Remainder" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
        int n = int.Parse(Console.ReadLine());
        double p1 = 0.0;
        double p2 = 0.0;
        double p3 = 0.0;
        for (int i = 0; i < n; i++) {
        int num = int.Parse(Console.ReadLine());
        if (num % 2 == 0) p1++;
        if (num % 3 == 0) p2++;
        if (num % 4 == 0) p3++;
        }
        var resultP1 = (p1 / n) * 100;
        var resultP2 = (p2 / n) * 100;
        var resultP3 = (p3 / n) * 100;
        // TODO: Print the result
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads n and n numbers
* Finds in percentage how many of them can divide without remainder at 2, 3 and 4
* Prints percentages p1, p2 and p3, formatted to the second digit
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3<br>3<br>6<br>9|33.33%<br>100.00%<br>0.00%|
|3<br>4<br>6<br>3|66.67%<br>66.67%<br>33.33%|
[/slide]

[slide]
# Problem: Vowel Sum
[code-task title="Vowel Sum" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads n - the count of characters:
* If character is vowel adds its value to the result

    |character|a|e|i|o|u|
    |---------|-|-|-|-|-|
    |value|1|2|3|4|5|

* Prints the result
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2<br>a<br>g|1|
|2<br>i<br>u|8|
[/slide]

[slide]
# Solution: Vowel Sum
[code-task title="Vowel Sum" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
        int n = int.Parse(Console.ReadLine());
        int vowelSum = 0;
        for (int i = 0; i < n; i++) {
        char letter = char.Parse(Console.ReadLine());
        switch (letter)
        {
            case 'a': vowelSum += 1; break;
            case 'e': vowelSum += 2; break;
            // TODO: Add the other cases
        }
        }
        Console.WriteLine(vowelSum);
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads n - the count of characters:
* If character is vowel adds its value to the result

    |character|a|e|i|o|u|
    |---------|-|-|-|-|-|
    |value|1|2|3|4|5|

* Prints the result
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2<br>a<br>g|1|
|2<br>i<br>u|8|
[/slide]

[slide]
# Problem: Rollercoaster
[code-task title="Rollercoaster" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads rollercoaster places, minimum age, count of people on the queue and age for each person
* If all places are taken, prints - "The rollercoaster departures"
* In other case, prints "Waiting..."
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1<br>10<br>1<br>15|The rollercoaster departures|
[/slide]

[slide]
# Solution: Rollercoaster
[code-task title="Rollercoaster" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
        int rollercoasterPlaces = int.Parse(Console.ReadLine());
        int minAge = int.Parse(Console.ReadLine());
        int peopleCount = int.Parse(Console.ReadLine());
        int validPeopleCount = 0;
        for (int i = 0; i < peopleCount; i++) {
        int personAge = int.Parse(Console.ReadLine());
        if (personAge >= minAge 
            && rollercoasterPlaces > validPeopleCount)
            validPeopleCount++;
        } 
        // TODO: Print the result
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads rollercoaster places, minimum age, count of people on the queue and age for each person
* If all places are taken, prints - "The rollercoaster departures"
* In other case, prints "Waiting..."
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1<br>10<br>1<br>15|The rollercoaster departures|
[/slide]

[slide]
# Problem: Multiply
[code-task title="Multiply" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads n 
* Prints n's multiples in the format "{n} x {i} = {result}"
* Where i are the numbers from 1 to 10 (inclusive)
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1|2 x 1 = 2<br>2 x 2 = 4<br>2 x 3 = 6<br>2 x 4 = 8<br>2 x 5 = 10<br>2 x 6 = 12<br>2 x 7 = 14<br>2 x 8 = 16<br>2 x 9 = 18<br>2 x 10 = 20|
[/slide]

[slide]
# Problem: Multiply
[code-task title="Multiply" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
        int n = int.Parse(Console.ReadLine());
        for (int i = 1; i <= 10; i++)
        {
        int result = n * i;
        Console.WriteLine($"{n} x {i} = {result}");
        }
    }
}
```
[/code-editor]
[task-description]
Write a program, which: 

* Reads n 
* Prints n's multiples in the format "{n} x {i} = {result}"
* Where i are the numbers from 1 to 10 (inclusive)
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1|2 x 1 = 2<br>2 x 2 = 4<br>2 x 3 = 6<br>2 x 4 = 8<br>2 x 5 = 10<br>2 x 6 = 12<br>2 x 7 = 14<br>2 x 8 = 16<br>2 x 9 = 18<br>2 x 10 = 20|
[/slide]