[slide]
# Break Operator
Used for prematurely **exiting** the loop

Can only be executed from the loop's **body**

When it is executed, the code inside the loop's body after it **is skipped** and does not execute

```csharp
while (true)
{
  int number = int.Parse(Console.ReadLine());
  if (number % 2 != 0)
  {
    break;
  }
  Console.WriteLine("Enter an even number!");
}
```
[/slide]