[slide]
# Comparison Operators
|Operators|Designation|
|---------|-----------|
| Equal to | == |
| Not Equal to | != |
| Greater than | > |
| Greater than or equal to | >= |
| Less than | < |
| Less than or equal to |  <= |
[/slide]

[slide]
# Value Comparison
In programming we can **compare** values

  * The result of the logical expressions is either ***true*** or ***false***

```csharp
int a = 5;
int b = 10;
Console.WriteLine(a < b);      // true
Console.WriteLine(a > 100);    // false
Console.WriteLine(a <= 5);     // true
Console.WriteLine(b == 2 * a); // true
Console.WriteLine(a != b);     // true
```
[/slide]

[slide]
# String Comparison
Comparing text using the equality operator(**==**)

```csharp
string a = "Examplе";
string b = a;
Console.WriteLine(a == b); // true
```
```csharp
string a = "hello";
string b = "hello";
Console.WriteLine(a == b); // true
Console.WriteLine(a < b); // error
```
[/slide]