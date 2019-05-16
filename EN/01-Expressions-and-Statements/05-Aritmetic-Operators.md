[slide]
# Arithmetic Operators: + and -
Adding numbers (operator + )

```csharp
int a = 5;
int b = 7;
int sum = a + b;
Console.WriteLine(sum); // 12 
```
Subtracting numbers (operator - )

```csharp
int a = 15;
int b = 7;
Console.WriteLine(a - b); // 8
```
[/slide]

[slide]
# Arithmetic Operators: * and /
Multiplying numbers (operator *)

```csharp
int a = 5;
int b = 7;
Console.WriteLine(a * b); // 35
```
Dividing numbers (operator / )

```csharp
int a = 25;
Console.WriteLine(a / 4); // 6
Console.WriteLine(a / 4.0); // 6.25
```
[/slide]

[slide]
# Arithmetic Operators: Division Behavior in C#
When **dividing integers**, the result is also integer:

```csharp
var a = 25;
Console.WriteLine(a / 4);  // Integer result: 6
Console.WriteLine(a / 0);  // Error: division by 0
```
When **dividing floating-points**, the result is also floating-point:

```csharp
var a = 15;
Console.WriteLine(a / 2.0); // 7.5
Console.WriteLine(a / 0.0); // Infinity
Console.WriteLine(0 / 0.0); // NaN
```
[/slide]

[slide]
# Arithmetic Operators: %
Modulo / remainder from integer division (operator **%** )

```csharp
int a = 7;
int b = 2;
Console.WriteLine(a % b);   // 1
```
```csharp
Console.WriteLine(3 % 2);   // 1
Console.WriteLine(4 % 2);   // 0
Console.WriteLine(3.5 % 1); // 0.5
```
[/slide]