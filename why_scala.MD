# 1. why scala

This chapter covers
>* What Scala is
>* High-level features of the Scala language
>* Why you should pick Scala as your next language

本章涵盖了
>* scala是什么
>* scala的高级特性
>* 为什么你应该选择scala做为你的下一个语言

Scala is a general-purpose programming language that runs on Java Virtual Machine (JVM) and .NET platforms. But the recent explosion of programming lan-guages on JVM, .NET, and other platforms raises a question that every developer faces today: which programming language to learn next? Which languages are ready for mainstream development? Among the heap of programming languages like Groovy, Ruby, Clojure, Erlang, and F#, why should you learn Scala?

Scala是一个运行在JVM和.NET平台上的general-purpose(通用)语言。但是今天，在极速增长的JVM、.NET和其它平台上的开发者们要面对的问题有：接下来要学习哪个编程语言?哪些语言会成为主流开发语言? 在一堆编程语言如Groovy，Ruby，Clojure，Erlang，和F#中，为什么你应该学习scala?

Learning a new language is merely a beginning. To become a useful and pro-ductive developer, you also need to be familiar with all the toggles and gizmos that make up the language infrastructure.

学习一个新语言只是一个开始。要成为有用并有成效的程序员，你还需要熟悉所有组成语言基础的toggles和gizmos。

Before I make the case for why Scala should be your next programming language, it’s important to understand what Scala is. It’s a feature-rich language that’s used in various types of applications, starting with building a large messaging layer for social networking sites such as Twitter to creating an application build tool like SBT2 (Simple Build Tool). Because of this scala-bility, the name of the language is Scala.

在这之前我给你一个案例告诉你为什么scala应该是你下一个编程语言，重要的是理解scala是什么。它是一个功能丰富的语言，那就可以用在很多类型的application上，开始构建一个如Twitter一样的社交网站大型消息层，使用SBT.因为这是scala-bility的，这也是这个语言名称的由来

This chapter explores the high-level features of the language and shows how they compare to the programming languages you may be very familiar with. This will help you to choose Scala as your next programming language.

这章探讨scala语言的高级特性以及展示与你其它可能会很熟悉的语言的不同。这将帮助你选择scala成为你的下一个编程语言。

If you’re an object-oriented programmer, you’ll quickly get comfortable with the language; if you’ve used a functional programming language, Scala won’t look much different because Scala supports both programming paradigms. Scala is one of those rare languages that successfully integrates both object-oriented and functional lan- guage features. This makes Scala powerful because it gives you more in your toolbox to solve programming problems. If you have existing Java applications and are looking for a language that will improve your productivity and at the same time reuse your existing Java codebase, you’ll like Scala’s Java integration and the fact that Scala runs on the JVM platform.

如果你是一个面向对像的开发者。你将会很快的适应scala;如果你正在使用一种函数式编程语言，scala并没有什么不同因为scala对这两种编程范式(programming paradigms)都支持。scala是那些为数不多的，成功的集成了面向对像和函数式两种语言特性的语言之一。这让scala变的很强大，因为它给你更多的工具来解决你在编程中遇到的问题。如果你有现成的java应用并且你正在寻找一种语言来提高你的编程效率同时要可以重用你已经存在的java代码，你将会喜欢scala与java的集成和scala运行在JVM平台上。

