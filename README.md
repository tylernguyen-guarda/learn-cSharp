Learn .net and C#

---Installing c# and c# sdk---

---Creating a .net project ---
1. Through VSCode (cmd+shift+p > project template > select template) >>> debug and run
2. through console navigate to correct dir then >>> (dotnet new console) >>> dotnet run


-----Microsoft Course: Write your first C# code------
https://learn.microsoft.com/en-us/collections/yz26f8y64n7k07

--Module 1:--
---Console.Write & Console.WriteLine---
The difference between Console.Write and Console.WriteLine

To print an entire message to the output console, you used the first technique, Console.WriteLine(). Adds a \n at the end of the literal string being written

To print to the output console, but without adding a line feed at the end, you used the second technique, Console.Write(). So, the next call to Console.Write() prints another message to the same line.

---Compiler---
A special program called a compiler converts your source code into a different format that the computer's central processing unit (CPU) can execute. 
When you used the green Run button in the previous unit, the code you wrote was first compiled, then executed.

Why does code need to be compiled? Although most programming languages seem cryptic at first, they can be more easily understood by humans than the computer's preferred language. 
The CPU understands instructions that are expressed by turning thousands or millions of tiny switches either on or off. Compilers bridge these two worlds by translating your human-readable instructions into a computer-understandable set of instructions.

---Breaking Down Console.WriteLine("Hello World"); ---
1. characters / line inside double "" == Literal String
2. "Console" == Class || WriteLine() == method 
2a. Methods always have  () after they are called . Some methods have input parameters, other do not . TO INVOKE , YOU MUST CALL () after method
3. semicolon ; is terminator

example:
Console.WriteLine("This is the first line.");
Console.Write("This is ");
Console.Write("the second line.");


--Module 2: Store and retrieve data using literal and variable values in C#--

---Exercise: Print Literal values---
example: Console.WriteLine('b');  (prints: b) (uses single quotes)

Single quotes created a character literal ; only used for singular char (TYPE)
Double quotes creates a string (TYPE)