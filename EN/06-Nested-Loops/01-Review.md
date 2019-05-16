[slide]
# While Loop
Control flow **statement** that allows code to be executed repeatedly based on a given **Boolean** condition

```csharp
while /*<-Keyword*/ (condition)
{
   // Body of the loop
}
```
**Example**

Print numbers from **1 to 5**

```csharp
int i = 1;
while (i <= 5)
{
   Console.WriteLine(i);
   i++;
}
// 1
// 2
// 3
// 4
// 5
```
[/slide]

[slide]
# While or For
***While*** and ***for*** loop help to **repeat** block of **code**

Use ***for*** when you know the **number of repetitions**

Use ***while*** when you don't know when the **end condition** will be met

[/slide]

[slide]
# The Break Operator
Used for **prematurely exiting** the loop

Can only be executed from the **body**, during an **iteration of the loop**

When ***break*** is executed the code in the loop's body after it **is skipped**

[/slide]