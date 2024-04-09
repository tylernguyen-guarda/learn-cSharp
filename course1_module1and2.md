Microsoft: Write your first code Using C#


-----Microsoft Course: Write your first C# code------
https://learn.microsoft.com/en-us/collections/yz26f8y64n7k07

--Module 2:--
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

Just like the string data type, you use char whenever you have a single alphanumeric character for presentation (not calculation).

---Use Integer Literals (int literal)---
- Numeric , WHOLE numbers (NO fractions)
- int requires no operators like the string or char

---Use Floating-point Literals---
- C# supports three data types for decimals (float, double  decimal)

--float (f or F) == ~6-9 digits 
-Console.WriteLine(0.25F); 
Least Precise

--double == ~15-17 digits
-Console.WriteLine(2.625);
Defaults to double when decimal entered without f or F

--decimal 28-29 digits
-Console.WriteLine(12.39816m);
Use m or M as literal suffix for decimal


---Use Boolean Literals---
-True or False

Console.WriteLine(true); (return True)
Console.WriteLine(false); (return False)

---Data Types Define Capabilities---
- If you need to perform a mathematical operation on numeric values, you should use an int or decimal. If you have data that is used for presentation or text manipulation, you should use a string or char data type.
-Example of String: Phone Number (you do not need to run any calculations )

-string for words, phrases, or any alphanumeric data for presentation, not calculation
-char for a single alphanumeric character
-int for a whole number
-decimal for a number with a fractional component
-bool for a true/false value




---Declare Variables---

A variable is a container for storing a type of value

variable name is  a human-friendly label the compuiler assigns to memory address
- When you want to store or change a value in that memory address, or whenever you want to retreive the stored value, you just use the variable name

Create / Declare Variable

string firstName;
- This can now store ONLY str values

--Rules and Conventions for variable name--
-Variable names can contain alphanumeric characters and the underscore character. Special characters like the hash symbol # (also known as the number symbol or pound symbol) or dollar symbol $ are not allowed.
-Variable names must begin with an alphabetical letter or an underscore, not a number.
-Variable names are case-sensitive, meaning that string Value; and string value; are two different variables.
-Variable names must not be a C# keyword. For example, you cannot use the following variable declarations: decimal decimal; or string string;.
-Variable names should use camel case, which is a style of writing that uses a lower-case letter at the beginning of the first word and an upper-case letter at the beginning of each subsequent word. For example, string thisIsCamelCase;.
-Variable names should begin with an alphabetical letter. Developers use the underscore for a special purpose, so try to not use that for now.
-Variable names should be descriptive and meaningful in your app. Choose a name for your variable that represents the kind of data it will hold.
-Variable names should be one or more entire words appended together. Don't use contractions or abbreviations because the name of the variable (and therefore, its purpose) may be unclear to others who are reading your code.
-Variable names shouldn't include the data type of the variable. You might see some advice to use a style like string strValue;. That advice is no longer current.


---Excercise 2 : Setting and getting value from variables

1. string firstName;
firstName = "Bob";

2. retrieve value stored in variable
Console.WriteLine(firstName);

Alternate method to write this:

string firstName = "Bob";
Console.WriteLine(firstName);


---Declare Implicitly Typed Local variables---

create implicit typed local variable using VAR
- var message = "Hello World";
The var keyword tells the C# compiler that the data type is implied by the assigned value. After the type is implied, the variable acts the same as if the actual data type had been used to declare it. The var keyword is used to save on keystrokes when types are lengthy or when the type is obvious from the context.

variables using var MUST be initialized / set upon creation

As you get started, it is recommended that you continue to use the actual data type name when you declare variables until you become more comfortable working with code. Using the data type when you declare variables will help you be purposeful as you write your code.

--Challenge: Display Literal and variable values--

-string firstName = "Bob";
-int numMessages = 3;
-var temp = 34.4;

-Console.Write("Hello, " + firstName + "! ");
-Console.Write("You have " + numMessages + " messages in your inbox. ");
-Console.Write("The temperature is " + temp +" celsius");