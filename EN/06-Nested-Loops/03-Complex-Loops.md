[slide]
# Complex Loops
Loops with different **steps**

```csharp
for (int i = n; i >= 1; i--) 
for (int j = 1; j <= n; j+=2)
for (int k = 1; k <= n; k*=2)
```
[/slide]

[slide]
# Problem: Numbers from N to 1
[code-task title="Numbers form N to 1" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads an integer number **n**
* Prints the numbers from **n** to **1** 
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|100|100<br>99<br>98<br>...<br>1|
|4|4<br>3<br>2<br>1|
[/slide]

[slide]
# Solution: Numbers from N to 1
[code-task title="Numbers form N to 1" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
        int n = int.Parse(Console.ReadLine());
        for (int i = n; i >= 1; i--) 
        {
            Console.WriteLine(i);
        }
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads an integer number **n**
* Prints the numbers from **n** to **1** 
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|100|100<br>99<br>98<br>...<br>1|
|4|4<br>3<br>2<br>1|
[/slide]

[slide]
# Problem: Numbers from 1 to N with Step 3
[code-task title="Numbers from 1 to N with Step 3" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads an integer number **n**
* Prints the numbers from **1** to **n** with step **3**
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|10|1<br>4<br>7<br>10|
|7|1<br>4<br>7|
[/slide]

[slide]
# Solution: Numbers from 1 to N with Step 3
[code-task title="Numbers from 1 to N with Step 3" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
        int n = int.Parse(Console.ReadLine());
        for (int i = 1; i <= n; i += 3) 
        {
            Console.WriteLine(i);
        }
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads an integer number **n**
* Prints the numbers from **1** to **n** with step **3**
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|10|1<br>4<br>7<br>10|
|7|1<br>4<br>7|
[/slide]

[slide]
# Problem: Even Powers of 2
[code-task title="Even Powers of 2" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads a number **n**
* Prints the even powers of 2 to 2**n**: 20, 22, 24, 28, …, 2n
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|10|1<br>4<br>16<br>...<br>1024|
|7|1<br>4<br>16<br>...<br>64|
[/slide]

[slide]
# Solution: Even Powers of 2
[code-task title="Even Powers of 2" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
        int n = int.Parse(Console.ReadLine());
        int num = 1;
        for (int i = 0; i <= n; i += 2)
        {
            Console.WriteLine(num);
            num = num * 2 * 2;
        }

    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads a number **n**
* Prints the even powers of 2 to 2**n**: 20, 22, 24, 28, …, 2n
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|10|1<br>4<br>16<br>...<br>1024|
|7|1<br>4<br>16<br>...<br>64|
[/slide]