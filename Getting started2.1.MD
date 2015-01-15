## 2.1 REPL with Scala interpreter

The easiest way to get started with Scala is by using the Scala interpreter, an interactive
shell for writing Scala expressions and programs. To start the Scala interpreter in
interactive mode, type scala at the command prompt. If everything goes fine with
your installation, you’ll see something like the following:

Welcome to Scala version 2.10.0.final (Java ...).
Type in expressions to have them evaluated.
Type :help for more information.
scala>

学习scala最简单的方式就是使用scala解析器（interpreter?）,这是一种交互式shell窗口，可以在上面允许scala表达式和scala程序，在命令行里敲击scala并按回车，就可以在交互模式下使用scala解析器（interpreter），如果之前你安装scala一切顺利的话你将会看下下列输出

Welcome to Scala version 2.10.0.final (Java ...). <br>
Type in expressions to have them evaluated. <br>
Type :help for more information.<br>
scala>

This means your Scala installation is successful. I’m running Scala version 2.10.0, and
all the code examples should work for this version and above. At the Scala prompt
type 42 and press Enter, and you should see something like this:

scala> 42
res0: Int = 42

这代码你scala安装成功了，我运行的scala版本是2.10.0，之后的代码案例都将在这个版本上运行。在scala提示符钱输入42，然后按回车，你会看到下列输出

scala> 42 <br>
res0: Int = 42

The first line is what you typed. The Scala interpreter reads the input 42, evaluates it
as an integer literal, creates an Int type object representing the number 42, and prints
it back to the console. res0 is the name of the variable created by the Scala interpreter
(the name of the variable could be different for you because the variable name is gen-
erated by the Scala interpreter at runtime) and it holds the value 42. If you type the
variable name, in this case res0, at the prompt, you’ll get similar output:

scala> res0 <br>
res1: Int = 42

第一行是你刚刚输入的，scala解析器读到输入为42，计算为整数字符，创建了个Int类型表示这个数字42，并打印在了控制台。
res0是scala解析器创建的变量名，（因为scala解析器是在运行时自动生成的这个变量，所以肯能这个变量和你的不一样），这个变量持有数字42的值。
如果你在提示符上敲入变量名，例如变量res0，你会得到一模一样的输出

scala> res0 <br>
res1: Int = 42

These steps together are called read-evaluate-print loop (REPL). You could loop read-
evaluate-print steps repeatedly inside the Scala interpreter. Now you’ll write your first
“Hello world” program in Scala:

scala> println("Hello world") <br>
Hello world

这些步骤的综合叫做 读-计算-打印 循环（REPL）。你将在scala解析器上重复的运行 读-计算-打印 步骤，现在开始使用scala写你的第一个hello world程序：

scala> println("Hello world") <br>
Hello world

You’re evaluating the println function by passing the "Hello world" string as a
parameter, and Scala outputs the same string.

你将字符串参数“hello world”传入 println函数中jisuan，scala会输出同样的字符串

>DEFINITION println is a function defined in scala.Console, which in turn
uses System.out.println to print messages to the console. Scala Predef
(part of the standard library) maps println to Console.println for you so
you don’t have to prefix it with Console when using it.

>定义：println 是一个在 scala.Console中定义的函数，依次使用System.out.println 打印信息到控制台，scala为你的预定义（标准库的一部分）println对应到Console.println。所以你在使用的时候不必加上Console前缀

In chapter 1, I mentioned that Scala integrates well with Java but didn’t provide an
example. I’ll fix that now:

scala> val myList = new java.util.ArrayList[String]() <br>
myList: java.util.ArrayList[String] = []

在第一章，我提到过scala可以和java很好的整合，但是当时缺少一个案例，现在我补上

scala> val myList = new java.util.ArrayList[String]() <br>
myList: java.util.ArrayList[String] = []

In this case you’re creating an instance of java.util.ArrayList that will hold
String-type objects. If you don’t remember all the methods that you could possibly
invoke on myList, don’t worry because the Scala interpreter will help you with that.
Type in myList, followed by a period, and press Tab; the Scala interpreter lists all the
methods you can invoke. Not only does it list all the methods associated with a data
type, it also autocompletes variable names and class names that are known to the
interpreter. I encourage you to spend some time with the Scala interpreter, explore
the available options, and keep it handy when working through the examples in this
book. Consider REPL as an essential part of learning a new language because it gives
quick feedback. Table 2.1 explains the REPL options available to you.

这里你创建了一个存储字符串类型的java链表，如果你记不清全部的方法，你可以反射调用mList对象。不用担心，scala解析器会帮助你的，敲入mList，等一会，然后敲入Tab；scala解析器会列举出所有你能反射到的方法，它不仅列出含有数据类型的方法，还自动补全了解析器反射到的变量名和类名，在学习这边书期间，我鼓励你花些时间使用scala解析器，去探索各种各样的选项。考虑到REPL是学习一门新语言必须的部分，因为他能很快的给到反馈，列表2.1解释了各种REPL的选项给你

###Table 2.1 Important Scala interpreter commands <br>
>* command :help <br> 
This command prints the help message with all the commands available in the Scala interpreter. 

命令 help 打印scala解析器所有命令的帮助信息

>* :cp <br>
Use this command to add a JAR file to the classpath for the Scala interpreter.
For example, :cp tools/junit.jar will try to find a JUnit JAR file relative to your
current location and, if found, it will add the JAR file to your classpath so that you can
refer to the classes inside the JAR file.

使用这个命令添加一个jar包到你的scala编译器的classpath目录，例如 ：cp tools/junit.jar 会在你的当前路径下寻找 JUnit JAR，如果找到了就会将该JAR添加到你的classpath下面，这样你就可以使用这个JAR包里的class 了

>* :load or :l <br>
Allows you to load Scala files into the interpreter. If you want to investigate existing
Scala code, you could load the file into the Scala interpreter, and all the definitions will
be accessible to you.

这两个命令允许你加载scala文件到解析器，如果你想研究现有的scala代码，你可以将这个代码文件加载到解析器，然后你可以看到所有的定义

>* :replay or :r <br>
Resets the interpreter and replays all the previous commands.

重启解析器，并运行所以之前运行过的命令

>* :quit or :q <br>
Exits the interpreter.

推出解析器

>* :type <br>
Displays the type of an expression without evaluating it. For example, :type 1 + 2 will
determine the type of the expression to Int without performing the add operation.

不计算，只显示表达式的类型，例如 type 1+2 会决定表达式的类型为Int 但是不计算加运算



