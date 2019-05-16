[slide]
# Nested Conditions

An ***if...else*** statement can exist within another ***if...else*** statement
  
Generally used when we have to test one condition followed by another

```csharp
if (expression)
{
  if (nested expression)
    // Code to be executed
  else
    // Code to be executed
}
```

**Logical Operators**

Logical operators are used to perform logical operation such as AND, OR

The logical operators are:

* AND (&&)

* OR (||)

* Logical negation (!)

**Switch-case**

Used for choosing among a list of possibilities

Alternative to an if-else statement

```csharp
switch (selector)
{
  case someCase:
    statements;
    break;
  default:
    statements;
    break;
}
```
[/slide]