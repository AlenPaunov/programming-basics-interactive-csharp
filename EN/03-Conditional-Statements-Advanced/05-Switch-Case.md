[slide]
# The Switch-Case Statement
Used for choosing among a list of possibilities

Alternative to an ***if-else*** statement

```csharp
switch (selector)
{
  case value1:
    statements;
    break;
  default:
    statements;
    break;
}
```
Example

```csharp
string choice = Console.ReadLine();
switch (choice)
{
  case "Y":
    Console.WriteLine("Yes");
    break;
  case "N":
    Console.WriteLine("No");
    break;
  default:
    Console.WriteLine("Invalid response");
    break;
}
```
[/slide]