[slide]
# Multiple Labels
Same logic has for more than one case

```csharp
switch (selector) {
  case value1:
  case value2:
    statements;
    break;
  default:
    statements; 
    break;
}
```

Example

```csharp
string animal = Console.ReadLine();
switch (animal) {
  case "dog":
  case "cat":
    Console.WriteLine("mammal");
    break;
  default:
    Console.WriteLine("unknown"); 
    break;
}
```
[/slide]