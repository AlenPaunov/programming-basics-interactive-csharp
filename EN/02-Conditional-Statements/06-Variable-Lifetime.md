[slide]
# Variable Scope
The block (range), in which a variable can be used:

```csharp
if (Console.ReadLine() == "Monday")
{
  double salary = double.Parse(Console.ReadLine());
}
Console.WriteLine(salary); // Compile-time error!
// The variable salary exists only in the block of code after the if statement
```
[/slide]