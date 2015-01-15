# 2. Getting started

This chapter covers
>* Working with the Scala REPL
>* Scala basics
>* For-comprehensions and pattern matching
>* Building a complete REST client in Scala

本章涵盖了
>* 使用 scala REPL
>* scala 基础
>* scal 表达式 和模式匹配（For-comprehensions 是scala中的一种数据结构，它允许直接遍历数组、列表、迭代器等数据结构而无需使用索引 ）
>* 使用scala构建一个完整 REST 客户端

In chapter 1 you learned what Scala is and how it compares to other programming
languages. I described the concepts at a high level, and in the next few chapters
you’re going to revisit those concepts and explore them in detail using examples. In
this chapter you learn about the basic Scala types, functions, for-comprehensions,
pattern matching, and the other usual suspects

在第一章 你了解了什么是scala以及它和其他编程语言的对比。
我从一个高的层面描述这些概念，在剩余的章节里，你将会复习到这些概念，并在详细的案例里探索它们。
在这一章节，你将学到scala 基本类型，函数，表达式，模式匹配，和其他常用的技巧

Some of the concepts in this chapter, like pattern matching and for-
comprehensions, are functional programming concepts. But because Scala is a
multi-paradigm language, I cover them with the rest of the nonfunctional program-
ming concepts. The objective of this chapter is for you to become comfortable with
the basics of the Scala language and its environment so you can start writing Scala
programs. Early on, I focus on only the Scala interpreter and its REPL environment
(you’ll see it in the next section) to keep things simple.

这个章节的一些观念是函数式编程的观念，例如模式匹配和scala表达式，
但是因为scala是一种混合语言，我将他们掩饰为剩余的非函数式编程观念。
这章的目标是在你开始学习scala的时候能舒服的使用scala语言和scala环境，
前面几节为简单起见，我只关注scala的解析器（interpreter？）和他的REPL环境（在后面的部分你会看到）

Before going any farther, make sure your Scala installation is working. Throughout
the chapter you’re going to work with various Scala examples, and it would be better if
you tried them in the Scala interpreter at the same time. Now let’s have some fun with
the Scala interpreter.

在开始之前，确保你已经安装好scala，
然后在这章你将学到很多scala案例，更好的是你可以同时在scala的解析器（interpreter？）上实验他们。现在让我们愉快的使用scala 解析器（interpreter？）玩耍吧

