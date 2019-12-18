# Coding Tips


Want to know how to program faster so that you can deliver software faster? Sure, who doesn't? The internet is full of tips  for developers—hundreds, thousands, perhaps even millions of them. The problem is, there are far more out there than anyone has time to read, so I've boiled them down for you.


## The problem with "faster"

To code faster, one has to be efficient; that is, no wasted effort or motion. This can mean everything from typing to tools to thinking. But most of our work as programmers isn’t typing, or compiling—it’s thinking. To think faster, you have to learn more patterns and relationships. This is the knowledge and wisdom that experience builds. What you need to go faster will change over time.

## The problem with "tips"

Most of the tips I read only apply at certain points along my journey, and don't necessarily apply to everyone. Many of these fall into the “personal journey” or  “what worked for me” categories. But my path is probably not your path. While some of the mechanical things that work for me will probably work for you, many of the domain and pattern choices I made may be of no use.

The mechanical stuff is pretty easy to optimize; the options are limited. But the learning stuff has no limits. No one will ever know it all. You must make strategic and tactical choices, and be prepared to take advantage of opportunities when they arise.

The utility of tips falls off as a function of specificity. The more specific tips don’t apply to everyone, but general tips are too, well, general. They’re much more difficult to turn into action. So what do you really want when you say you want to "go faster?" I'll tell you.

[ Get up to speed with TechBeacon's Guide to Software Test Automation. Plus: Get the Buyer’s Guide for Selecting Software Test Automation Tools ]

## What you want is flow

What every programmer wants, especially in the era of DevOps, is flow. Flow state maximizes throughput and increases enjoyment by incorporating just the right level of challenge; one stays fully engaged in the moment and in the work (this is not to be confused with the Ballmer Peak). Sustaining flow state requires a suitable environment and frictionless process.

Flow state when pairing is like each of you having an extra brain. Unfortunately, many developer environments, such as open offices, are unfriendly to flow.

## Your options may be limited

When you find something sub-optimal about your process, or yourself, the choices of how to address such constraints are limited:

* **Ignore it.**  Maybe it will get better on its own.

* **Avoid it.** Is it really necessary?

* **Automate it.** Make the machine do it.

* **Delegate it.** Rarely possible, this is passing the buck. But it is a legit option when available.

* **Grind it down.** We all have to do this from time to time (daily). Some  jobs are larger than others.

If your typing is slower than you’d like, take a little time and level up. If your integrated development environment is confusing and unhelpful (or perhaps too helpful), try something different or simpler. If you can’t get away from it, learn more about it; you may find another way, or at least learn the limits.

There are numerous ways to learn. Google is your friend, as are books, videos, blog posts, Stack Overflow questions, and, of course, other people. Some things you want to learn may be hidden; others may be larger than they appear. Balance benefit with effort and be patient with yourself. Celebrate every achievement and keep moving.

## Top tips for programming faster

One way of grouping and looking at the tips below is by applying a few high-level categories as a way to draw interesting generalizations from the collection:

* **Reflect.** What do you want, what do you actually do; includes measuring and optimization.

* **Flow.** No friction from tools, processes, environment, or knowledge; seek continual challenge but not too much.

* **Learn.** The fundamentals: languages, tools, patterns, practices, etc., from everyone (especially those willing to teach); learn how you learn, and learn continuously.

* **Teach.** Teach others. Having to explain things forces simplification, and the transformation from thoughts to verbal or visual expressions produces insights.

* **Express and explore.** Look outside your normal duties; draw, write, blog, go to meetups, attend and give presentations.


### Here are few more tips to code efficently in pyhton

* Indentation

Many a times it is required to treat more than one statements in a program as a block. Different programming languages use different techniques to define scope and extent of block of statements in constructs like class, function, conditional and loop. In C and C++ for example, statements inside curly brackets are treated as a block. Python uses uniform indentation to mark block of statements.

Before beginning of block symbol : is used. First and subsequent statements in block are written by leaving additional (but uniform) whitespace (called indent) . In order to signal end of block, the whitespace is dedented. Following example illustrates the use of indents in Python:

![example_image](/images/Indentation.png)


* Don't repeat yourself!

OF ALL THE PRINCIPLES OF PROGRAMMING, **Don’t Repeat Yourself (DRY)** is perhaps one of the most fundamental. The principle was formulated by Andy Hunt and Dave Thomas in The Pragmatic Programmer, and underlies many other well-known software development best practices and design patterns. The developer who learns to recognize duplication, and understands how to eliminate it through appropriate practice and proper abstraction, can produce much cleaner code than one who continuously infects the application with unnecessary repetition.

**Duplication Is Waste**Every line of code that goes into an application must be maintained, and is a potential source of future bugs. Duplication needlessly bloats the codebase, resulting in more opportunities for bugs and adding accidental complexity to the system. The bloat that duplication adds to the system also makes it more difficult for developers working with the system to fully understand the entire system, or to be certain that changes made in one location do not also need to be made in other places that duplicate the logic they are working on. DRY requires that “every piece of knowledge must have a single, unambiguous, authoritative representation within a system.”


* Class


Classes provide a means of bundling data and functionality together. Creating a new class creates a new type of object, allowing new instances of that type to be made. Each class instance can have attributes attached to it for maintaining its state. Class instances can also have methods (defined by its class) for modifying its state.

Compared with other programming languages, Python’s class mechanism adds classes with a minimum of new syntax and semantics. It is a mixture of the class mechanisms found in C++ and Modula-3. Python classes provide all the standard features of Object Oriented Programming: the class inheritance mechanism allows multiple base classes, a derived class can override any methods of its base class or classes, and a method can call the method of a base class with the same name. Objects can contain arbitrary amounts and kinds of data. As is true for modules, classes partake of the dynamic nature of Python: they are created at runtime, and can be modified further after creation.

In C++ terminology, normally class members (including the data members) are public (except see below Private Variables), and all member functions are virtual. As in Modula-3, there are no shorthands for referencing the object’s members from its methods: the method function is declared with an explicit first argument representing the object, which is provided implicitly by the call. As in Smalltalk, classes themselves are objects. This provides semantics for importing and renaming. Unlike C++ and Modula-3, built-in types can be used as base classes for extension by the user. Also, like in C++, most built-in operators with special syntax (arithmetic operators, subscripting etc.) can be redefined for class instances.


* Object

Objects have individuality, and multiple names (in multiple scopes) can be bound to the same object. This is known as aliasing in other languages. This is usually not appreciated on a first glance at Python, and can be safely ignored when dealing with immutable basic types (numbers, strings, tuples). However, aliasing has a possibly surprising effect on the semantics of Python code involving mutable objects such as lists, dictionaries, and most other types. This is usually used to the benefit of the program, since aliases behave like pointers in some respects. For example, passing an object is cheap since only a pointer is passed by the implementation; and if a function modifies an object passed as an argument, the caller will see the change — this eliminates the need for two different argument passing mechanisms as in Pascal.

* Static

Static methods in Python are extremely similar to python class level methods, the difference being that a static method is bound to a class rather than the objects for that class.

This means that a static method can be called without an object for that class. This also means that static methods cannot modify the state of an object as they are not bound to it. Let’s see how we can create static methods in Python.

* Attribute 

Attributes may be read-only or writable. In the latter case, assignment to attributes is possible. Module attributes are writable: you can write modname.the_answer = 42. Writable attributes may also be deleted with the del statement. For example, del modname.the_answer will remove the attribute the_answer from the object named by modname.

Namespaces are created at different moments and have different lifetimes. The namespace containing the built-in names is created when the Python interpreter starts up, and is never deleted. The global namespace for a module is created when the module definition is read in; normally, module namespaces also last until the interpreter quits. The statements executed by the top-level invocation of the interpreter, either read from a script file or interactively, are considered part of a module called __main__, so they have their own global namespace. (The built-in names actually also live in a module; this is called __builtin__.)
