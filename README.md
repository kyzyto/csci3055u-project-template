# _Scala_

- _Adunife Kizito Okoye_
- _adunife.okoye@uoit.net_

## About the language
>  **History** 
>> - Created by Martin Odersky. 
>> - It was initially designed at the École Polytechnique Fédérale de Lausanne (EPFL) in the year 2001 and initially released in the year 2003, but it only surfaced to the public in the year 2004. Scala was originally released on the Java platform as a general-purpose programming language. 
>> - The name Scala is an abbreviation of "scalable" not some whimsical notion, it represents a language that is scalable according to the needs of its users.

>  **Some interesting features**
>> - Scala was designed to address critisims of Java
>> - Everything looks like an object
>> - Import statements can be anywhere
>> - Streams process big data (or infinite data) efficiently

## About the syntax

> _Scala could be executed in two modes: one is interactice mode and the another is script mode._
 >> - ### Interactive mode ###
 >>> To open scala in the command prompt use the following  command.
 >>>  ```
 >>>  \>scala
 
 >>> The following should be displayed if Scala is installed in your system.
 >>>  ```
 >>>  Welcome to Scala version 2.9.0.1
 >>>  Type in expressions to have them evaluated.
 >>>  Type :help for more information.
 
 >>>  Type the following text to the right of the Scala prompt and press the Enter key −
 >>>  ```
 >>>  scala> println("Hello, Scala!");
 
 >>>  The following result will be produced
 >>>  ```
 >>>  Hello, Scala!
 
 >> - ### Script mode ###
 >>> **HelloWorld**
 >>> ```scala
 >>>  object HelloWorld {
 >>>  /* This is my first java program.  
 >>>  * This will print 'Hello World' as the output
 >>>  */
 >>>  def main(args: Array[String]) {
 >>>      println("Hello, world!") // prints Hello World
 >>>  }
 >>> }
 
 >>>  The file is saved as **Helloworld.scala**
 >>>  Then open commmand promtpt and go to the directory where you saved the program
 Then '**scalac**' command is typed in fromt of the file **Helloworld.scala** in commmand prompt to compile the file.
 Since this is only bytecode whic will run in Java Virtual Machine (JVM) using '**scala**' command.
 >>>   ```
 >>>   \> scalac HelloWorld.scala
 >>>   \> scala HelloWorld
 
 >>>   The above command is used to compile and execute the Scala program. And output 
 >>>   ```
 >>>   Hello, World!
 
 >>> **Syntax and conding conventions**
 >>>> - **Case Sensitivity** − Scala is case-sensitive, which means identifier hello and Hello have completely different meanings in Scala.
 >>>> - **Class Names** − For all class names, the first letter should be in Upper Case. If several words are used to form a name of the class, each inner word's first letter should be in Upper Case.
 >>>> - **Program File Name** − Name of the program file should exactly match the object name. When saving the file you should save it using the object name (Remember Scala is case-sensitive) and append ‘.scala’ to the end of the name. (If the file name and the object name do not match your program will never compile). In essence if the object name is 'HelloWord' the file must be saved as 'HelloWorld.scala'
 >>>> - **def main(args: Array[String])** − Scala program processing starts from the main() method which is a mandatory part of every Scala Program.
 >>>> - **Method Names** − All method names must begin with a Lower Case letter. If multiple words are used to form the name of the method, then each inner word's first letter should be in Upper Case. For example ' def myMethodName() '
 >>>> - **Identifiers** - In Scala names are required for all components, and the names used for objects, methods, classes and  variables are called identifiers. Since Scala is case sensitive keywoords cannot be used and an identifier.
 >>>>> - **Operator Identifiers** - These kind of Identifiers consists of the printable ASCII characters such as +,-,?,: or #.And they could consist of one or more operator characters.
 >>>>>   ```
 >>>>>   + ++ ::: <?> :>
 >>>>> - **Alphanumeric Identifiers** - These kind of Identifiers could either start with a letter or and underscore, which other letters or underscore and digits could follow up. The the symbol '$" is restricted and should not be used in Scala as it is a reserved keyword.
 >>>>>   ```scala
 >>>>>   age, _value, salary, _1_value.
 >>>>> - **Literal Identifiers** - These are basically arbitrary string enclosed in back ticks (`...`)
 >>>>>   ```
 >>>>>   `x `<clinit>` `yield`
 >>>>> - **Mixed Identifiers** - A mixed identifier consists of an alphanumeric identifier, then an underscore and a operator identifier
 >>>>>   ```scala
 >>>>>   unary_+,  myvar_=
 
 >>> **Comments, Newline Characters, Blank Lines and Whitespace in Scala**
 >>>> - Comments - In Scala single-line and multiple-line comments are supported in a very similar way to Java. All characters available inside any comment are ignored by Scala compiler. So it is important that multi-line comments be nested, and are required to be nested properly.
 >>>> **HelloWorld**
 >>>> ```scala
 >>>>  object HelloWorld {
 >>>>  /* This is my first java program.  
 >>>>  * This will print 'Hello World' as the output
 >>>>  */
 >>>>  def main(args: Array[String]) {
 >>>>      println("Hello, world!") // prints Hello World
 >>>>  }
 >>>> }
 
 >>>> - Newline Characters - Since Scala is line-oriented language where statements may be terminated by semicolons (;) or newlines. It has a very similar approach to this like as that of Java
 >>>>   ```
 >>>>   val g = "hello"; println(g)
 >>>> - Blank Lines and Whitespace - In Scala lines containing only whitespace, could possibly be with a comment, is known as a blank line, and Scala totally ignores it while running the program. Tokens may be separated by whitespace characters and/or comments.
## About the tools

> _Describe the compiler or interpreter needed_.
>> - 
>> - 
>> - 
>> - 


## About the standard library

> _Give some examples of the functions and data structures
> offered by the standard library_.

## About open source library

> _Describe at least one contribution by the open source
community written in the language._

# Analysis of the language
>> **The style of programming supported by the language: functional vs procedural programming**
>>> _One of Scala’s perks is that its functional programming functionality with an OOP style._


>> **The ability to perform meta-programming such as macros**
>>> _Pattern matching in Scala is no joke. Scala uses the match statement for this purpose, which is a powerful version of Java's switch statement. It allows you to match on any type of data, lists, and even your own types. If you haven't already tried it, I suggest you play around with it a little._

>> **Symbol resolution and its support for closure**
>>> _Simple symbol resolutions are by far the most common. In this case, two symbols with similar characteristics are detected, with one symbol taking precedence over the other. This symbol resolution is carried out silently by the link-editor. For example, with symbols of the same binding, a symbol reference from one file is bound to a defined, or tentative symbol definition, from another file. Or, a tentative symbol definition from one file is bound to a defined symbol definition from another file. This resolution can occur between two relocatable objects, or between a relocatable object and the first definition found in a shared object dependency._

>>> _Symbols that undergo resolution can have either a global or weak binding. Within relocatable objects, weak bindings have lower precedence than global binding. Relocatable object symbols with different bindings are resolved according to a slight alteration of the basic rules. Weak symbols can usually be defined through the compiler, either individually or as aliases to global symbols._


>>> _Complex symbol resolutions occur when two symbols of the same name are found with differing attributes. In these cases, the link-editor generates a warning message, while selecting the most appropriate symbol. This message indicates the symbol, the attributes that conflict, and the identity of the file from which the symbol definition is taken. In the following example, two files with a definition of the data item array have different size requirements._

>> **Scoping rules supported by the language: lexical vs dynamic scoping**
>>> _The scoping rules supported by the language is lexical._

>> **Functional programming constructs either as part of the language or supported by the standard library of the runtime**

>>> _It allows you to interact seamlessly with standard Java libraries while developing from a functional perspective._


>> **Its type system: static vs dynamic types**
>>> _Scala is statically typed and compiles down to the same fast bytecode as Java so its usually about as fast as Java (sometimes a little faster sometimes a little slower). e.g. compare how well Scala does in some benchmarks with groovy or jruby. Or this. Note speed isn't everything - there are times when you might want to trade code thats 10x slower for more productivity and conciseness; but for a long term replacement for javac speed is important.
Yet Scala has type inference - so its typically as concise as Ruby/Groovy but that everything has static types. This is a good thing; it makes code comprehension, navigation & documentation much simpler. Any token/method/symbol you can click on to navigate to the actual implementation code & documentation. No wacky monkey patching involved, or doubting of who added a method, when and how - which is great for large projects with lots of folks working on the same code over long periods of time. Scala seems to hit the perfect sweet spot between the consise feel of a dynamic language, while actually being completely statically typed. So I never have to remember the magic methods that are available - or run a script in a shell then inspect the object to see what it really looks like - the IDE/compiler just knows while you edit._


>> **Strengths and weaknesses of the language**
>>> _Weakness_
>>>> - Slow Compilation- In the world of coding speed in very important and Scala is slow in comparison to Java and Kotlin, which runs in second where as it runs in seconds.
>>>> - Binary Compilation in Challenging- for a few versions. Let us say you compiled with Scala 2.11 the same would not compile with 2.1.
>>>> - Less Efficient in the Management of Null Safety._

>>> _Strength_
>>>> - Simple and straightforward syntax- Scala typically requires two-thirds less code than Java. The syntax is also more flexible. For example, you can leave out periods between method calls so the code is more human-readable and easier to understand.
>>>> - Inherently immutable objects- Scala’s programming language reduces many thread-safety concerns that spring up in traditional Java applications.
>>>> - Highly functional- Scala treats functions as first-class citizens.
>>>> - Fast implementation speed- It allows for quicker implementation and enhanced performance.
>>>> - It is fun- Scala challenges strong engineers in a meaningful and entertaining manner, making development more fun.
>>>> - Easy to solve concurrency issues. It has an Actor library to solve concurrency problems more rapidly.
>>>> - XML support. Scala supports XML, which is beneficial if you have a need to encode documents in your products._


