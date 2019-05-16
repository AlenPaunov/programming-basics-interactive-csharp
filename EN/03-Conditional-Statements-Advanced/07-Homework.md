[slide]
# Problem: Fruit or Vegetable
[code-task title="Fruit or Vegetable" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program to check for fruit or vegetable:

* Read a single input line: an item from the greengrocery
* Fruits: banana, apple, kiwi, cherry, lemon, grapes
* Vegetables: cucumber, pepper, carrot, onion
* Print: "vegetable", "fruit" or "unknown"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|lemon|fruit|
|carrot|vegetable|
[/slide]

[slide]
# Solution: Fruit or Vegetable
[code-task title="Fruit or Vegetable" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
        string product = Console.ReadLine();
        switch (product) {
        case "cucumber":
        case "pepper":
        case "carrot":
            Console.WriteLine("vegetable");
            break;
        // TODO: Implement the other cases
        }
    }
}
```
[/code-editor]
[task-description]
Write a program to check for fruit or vegetable:

* Read a single input line: an item from the greengrocery
* Fruits: banana, apple, kiwi, cherry, lemon, grapes
* Vegetables: cucumber, pepper, carrot, onion
* Print: "vegetable", "fruit" or "unknown"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|lemon|fruit|
|carrot|vegetable|
[/slide]

[slide]
# Problem: Day of Week
[code-task title="Day of Week" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program to print the day of week as words:

* Read and integer n: the day of the week in range [1..7]
* Print the name of the day (as words, in English)
* Print "Error" if the number is not in the given range
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1|Monday|
|8|Error|
|7|Sunday|
[/slide]

[slide]
# Solution: Day of Week
[code-task title="Day of Week" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
        int day = int.Parse(Console.ReadLine());
        switch (day)
        {
        case 1: Console.WriteLine("Monday"); break;
        case 2: Console.WriteLine("Tuesday"); break;
        // TODO: Implement the other valid days
        default: Console.WriteLine("Error"); break; 
        }
    }
}
```
[/code-editor]
[task-description]
Write a program to print the day of week as words:

* Read and integer n: the day of the week in range [1..7]
* Print the name of the day (as words, in English)
* Print "Error" if the number is not in the given range
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1|Monday|
|8|Error|
|7|Sunday|
[/slide]

[slide]
# Problem: Vowel or Consonant
[code-task title="Vowel or Consonant" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program to check a letter for vowel or consonant:

* Read a letter from the English alphabet
* Print either "Vowel" or "Consonant"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|a|Vowel|
|E|Vowel|
|b|Consonant|
[/slide]

[slide]
# Solution: Vowel or Consonant
[code-task title="Vowel or Consonant" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
        char letter = char.Parse(Console.ReadLine());
        if (letter == 'A' || letter == 'a' || 
            letter == 'E' || letter == 'e' || 
            letter == 'I' || letter == 'i' || 
            letter == 'O' || letter == 'o' || 
            letter == 'U' || letter == 'u')
            Console.WriteLine("Vowel");
        else
        Console.WriteLine("Consonant");
    }
}
```
[/code-editor]
[task-description]
Write a program to check a letter for vowel or consonant:

* Read a letter from the English alphabet
* Print either "Vowel" or "Consonant"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|a|Vowel|
|E|Vowel|
|b|Consonant|
[/slide]

[slide]
# Problem: Product of 3 Numbers
[code-task title="Product of 3 Numbers" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Calculate the sign of the product of 3 numbers:

* Read 3 floating-point numbers
* Print the sign of the product of the entered 3 numbers: positive, negative or zero

Try to do this without multiplying the 3 numbers

[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2<br>3<br>-1|negative|
|-3<br>-4<br>5|positive|
[/slide]

[slide]
# Solution: Product of 3 Numbers
[code-task title="Product of 3 Numbers" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
        // TODO: Read 3 real numbers – n1, n2 & n3
        if (n1 == 0 || n2 == 0 || n3 == 0)
        Console.WriteLine("zero");
        else
        {
        int negativeNumbersCount = 0;
        if (n1 < 0) negativeNumbersCount++;
        if (n2 < 0) negativeNumbersCount++;
        if (n3 < 0) negativeNumbersCount++;
        if (negativeNumbersCount % 2 == 0)
            Console.WriteLine("positive");
        else
            Console.WriteLine("negative");
        }
    }
}
```
[/code-editor]
[task-description]
Calculate the sign of the product of 3 numbers:

* Read 3 floating-point numbers
* Print the sign of the product of the entered 3 numbers: positive, negative or zero

Try to do this without multiplying the 3 numbers

[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2<br>3<br>-1|negative|
|-3<br>-4<br>5|positive|
[/slide]

[slide]
# Problem: Sorted Numbers
[code-task title="Sorted Numbers" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program, which checks for sorted 3 numbers:

* Read 3 real numbers
* Print "Ascending" if the numbers are in ascending order
* Print "Descending" if the numbers are in descending order
* Print "Not sorted" in any other case

[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1<br>2<br>3|Ascending|
|3<br>1<br>2|Not sorted|
[/slide]

[slide]
# Solution: Sorted Numbers
[code-task title="Sorted Numbers" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
        double n1 = double.Parse(Console.ReadLine());
        double n2 = double.Parse(Console.ReadLine());
        double n3 = double.Parse(Console.ReadLine());
        if (n1 < n2 && n2 < n3)
            Console.WriteLine("Ascending");
        else if (n1 > n2 && n2 > n3)
            Console.WriteLine("Descending");
        else
            Console.WriteLine("Not sorted");
    }
}
```
[/code-editor]
[task-description]
Write a program, which checks for sorted 3 numbers:

* Read 3 real numbers
* Print "Ascending" if the numbers are in ascending order
* Print "Descending" if the numbers are in descending order
* Print "Not sorted" in any other case

[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1<br>2<br>3|Ascending|
|3<br>1<br>2|Not sorted|
[/slide]

[slide]
# Problem: Vacation Expenses
[code-task title="Vacation Expenses" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program, which calculates vacation expenses:

* Read season, accommodation type and count of the days
* Print the total expenses, based on the price table bellow,formatted to the 2nd * digit after the decimal point

[/task-description]
[code-io /]
[/code-task]
|Season|Hotel|Camping|Discount|
|-----|------|-------|--------|
|Spring|30|10|20%|
|Summer|50|30|0%|
|Autumn|20|15|30%|
|Winter|40|10|10%|
# Sample Input and Output
|Input|Output|
|-----|------|
|Winter<br>Hotel<br>5|180.00|
[/slide]

[slide]
# Solution: Vacation Expenses
[code-task title="Vacation Expenses" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
        string season = Console.ReadLine();
        string accommodation = Console.ReadLine();
        int days = int.Parse(Console.ReadLine()); 
        if (season == "Spring") {
            if (accommodation == "Hotel")
                totalPrice = days * 30 * 0.70;
            else if (accommodation == "Camping")
                totalPrice = days * 10 * 0.70;
        }
        // TODO: Implement the other cases
    }
}
```
[/code-editor]
[task-description]
Write a program, which calculates vacation expenses:

* Read season, accommodation type and count of the days
* Print the total expenses, based on the price table bellow,formatted to the 2nd * digit after the decimal point

[/task-description]
[code-io /]
[/code-task]
|Season|Hotel|Camping|Discount|
|-----|------|-------|--------|
|Spring|30|10|20%|
|Summer|50|30|0%|
|Autumn|20|15|30%|
|Winter|40|10|10%|
# Sample Input and Output
|Input|Output|
|-----|------|
|Winter<br>Hotel<br>5|180.00|
[/slide]

[slide]
# Problem: Cinema
[code-task title="Cinema" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Calculate the price for all the tickets for a cinema movie:

* Reads the type of the movie, the rows and the seats per row in the cinema
* Prints the total price for all seats formatted to the 2nd digit after the decimal point

[/task-description]
[code-io /]
[/code-task]
|Type|Price|
|-----|----|
|Premiere|12.00|
|Normal|7.50|
|Discount|5.00|
# Sample Input and Output
|Input|Output|
|-----|------|
|Normal<br>12<br>9|810.00|
[/slide]

[slide]
# Solution: Cinema
[code-task title="Cinema" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
       string type = Console.ReadLine();
        int rows = int.Parse(Console.ReadLine());
        int cols = int.Parse(Console.ReadLine());
        int seats = rows * cols;
        switch (type) {
            case "Premiere":
                Console.WriteLine("{0:f2}", seats * 12.0);
                break;
            // TODO: Implement the other cases
        }
    }
}
```
[/code-editor]
[task-description]
Calculate the price for all the tickets for a cinema movie:

* Reads the type of the movie, the rows and the seats per row in the cinema
* Prints the total price for all seats formatted to the 2nd digit after the decimal point

[/task-description]
[code-io /]
[/code-task]
|Type|Price|
|-----|----|
|Premiere|12.00|
|Normal|7.50|
|Discount|5.00|
# Sample Input and Output
|Input|Output|
|-----|------|
|Normal<br>12<br>9|810.00|
[/slide]

[slide]
# Problem: Operations with Numbers
[code-task title="Operations with Numbers" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program to apply an operator for given two numbers:

* Read two real numbers and math operator from the console
* The math operator could be: "+", "-", "/", "%" and "*"
* The output should be in the following format: "\{N1\} \{operator\} \{N2\} = \{result\}"

[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|10<br>12<br>+|10 + 12 = 22|
[/slide]

[slide]
# Solution: Operations with Numbers
[code-task title="Operations with Numbers" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      double num1 = double.Parse(Console.ReadLine());
        double num2 = double.Parse(Console.ReadLine());
        string operation = Console.ReadLine();
        double result = 0;
        if (operation == "+") result = num1 + num2; 
        else if (operation == "-") result = num1 - num2;
        // TODO: Implement the remaining operations
        Console.WriteLine("{0} {1} {2} = {3}", num1, operation, num2, result);
    }
}
```
[/code-editor]
[task-description]
Write a program to apply an operator for given two numbers:

* Read two real numbers and math operator from the console
* The math operator could be: "+", "-", "/", "%" and "*"
* The output should be in the following format: "\{N1\} \{operator\} \{N2\} = \{result\}"

[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|10<br>12<br>+|10 + 12 = 22|
[/slide]

[slide]
# Problem: ATM
[code-task title="ATM" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program to simulate an ATM withdrawal:

* Read: balance, withdraw and limit
* Print "The withdraw was successful." if the balance is enough
* Print "The daily limit was exceeded." if the limit is exceeded
* Print "Insufficient availability." if the balance isn't enough

[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|420<br>20<br>25|The withdraw was successful.|
|10<br>50<br>20|The daily limit was exceeded.<br>Insufficient availability.|
[/slide]

[slide]
# Solution: ATM
[code-task title="ATM" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
        // TODO: Read the input numbers
        if (balance >= withdraw && withdraw <= limit)
            Console.WriteLine("The withdraw was successful.");
        if (withdraw > dailyLimit)
            Console.WriteLine("The daily limit was exceeded.");
        if (withdraw > balance)
            Console.WriteLine("Insufficient availability.");
    }
}
```
[/code-editor]
[task-description]
Write a program to simulate an ATM withdrawal:

* Read: balance, withdraw and limit
* Print "The withdraw was successful." if the balance is enough
* Print "The daily limit was exceeded." if the limit is exceeded
* Print "Insufficient availability." if the balance isn't enough

[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|420<br>20<br>25|The withdraw was successful.|
|10<br>50<br>20|The daily limit was exceeded.<br>Insufficient availability.|
[/slide]

[slide]
# Problem: Biggest of Five Numbers
[code-task title="Biggest of Five Numbers" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program to find the biggest among 5 numbers
* Read 5 integers
* Print the biggest number
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1<br>2<br>3<br>4<br>5|5|
|-1<br>-2<br>-3<br>-4<br>-5|-1|
[/slide]

[slide]
# Solution: Biggest of Five Numbers
[code-task title="Biggest of Five Numbers" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
        int num1 = int.Parse(Console.ReadLine());
        int num2 = int.Parse(Console.ReadLine());
        int num3 = int.Parse(Console.ReadLine());
        int num4 = int.Parse(Console.ReadLine());
        int num5 = int.Parse(Console.ReadLine());
        if (num1 >= num2 && num1 >= num3 && num1 >= num4 && num1 >= num5)
            Console.WriteLine(num1);
        // TODO: Implement the remaining cases
    }
}
```
[/code-editor]
[task-description]
Write a program to find the biggest among 5 numbers
* Read 5 integers
* Print the biggest number
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1<br>2<br>3<br>4<br>5|5|
|-1<br>-2<br>-3<br>-4<br>-5|-1|
[/slide]