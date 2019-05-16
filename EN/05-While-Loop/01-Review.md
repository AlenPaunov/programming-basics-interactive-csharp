[slide]
# Simple For Loop
Used for repeating the execution of a certain code a known number of times

The body of the loop **contains** a block with a source **code**,which is **executed** at each iteration

```csharp
for (initialization; condition; step)
{   
  // Body of the loop
}
```
**Example**

Print the numbers ***from 1 to 10***

```csharp
// keyword -> initialization -> condition ->  step
for (int i = 1; i <= 10; i++)
{
   Console.WriteLine(i); // Loop body
}
```
[/slide]

[slide]
# Prefix and Postfix
Pre-decrement

```csharp
int a = 1; 
Console.WriteLine(--a); // 0
Console.WriteLine(a);   // 0
```
Post-decrement

```csharp
int a = 1; 
Console.WriteLine(a--); // 1
Console.WriteLine(a);   // 0
```
[/slide]