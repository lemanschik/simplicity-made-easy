# simplicity-made-easy
A book about simple things that are maybe not as easy but simple in ECMAScript.

A person once suggested to me a talk and today i want to port that talk over to ECMAScript to improve the knowleg about ECMAScript Engines.
They in fact drive the world for good reason. They are simple and not easy. This book trys to get you familar with the != between simple and easy. 

the most easy example is maybe webpack it is a great fit as also typescript both are easy to use you install run adjust some config you are done. 

you created guard rails via tests and a test framework because why not drive against a wall before you hit your target?!?.

So lets show how easy the tools are just follow the docs round about 30 pages of small printed text so easy to grasp around right?

Ok so we are on page. 


lets explain now what they simple do:
- replace text in strings following conditional rules. As also break and error and simply stop working. they call that linting. 
- write the modified text in one or more files also copy some binary additional files.
- What else? i am not aware of something else prove me wrong. 

- the best typescript and webpack features are you never know if the error is caused by you or them that is a extra bonus you can easy look that up
  - start your debugger session and start investigating most best is when you also put electron into the chain then you add some extra complexity. 
  - hope you get what we are talking about here it is so easy right? lets use vscode which runs inside electron lets connect debuggers before that we read about 100 pages and the links they reference that was easy took us 1 week we found out ok it is a upstream error now we raise a issue in the upstream
  - then our employer told us we are fired because he has no money any more deadline not reached because used best tools and practices. 

does the above sound familar?

ok so i hope we are on page i did reduce the documentation of webpack and typescript now into 3 main parts they are simple but not easy.

so when we look now in one of the code bases lets take typescript as they show how easy it is to make simple mistakes. They use inheritence all over so they did the main failure of applying classes and structures around Data we call that ORM/OMG you can only do one thing with data in general. And that is ruin it so if you do not ruin the data you safed a lot of frustration on the long run.

If you want to manipulate data correct you need to use Streams they are internal managed Queue implementations so you do not need to code your own. They support everything that you need to build a complex system out of simple modules that you turn into composed components. So there was no term like easy! It is not easy! Easy would mean i give you one line of code and everything is done like webpack and typescript. 

The good news anywway is that the current ECMAScript API's are so well overdesigned that it is even easy to use them most time as beeing easy was one of the main goals of ECMAScript it self. So the need to add more easyness is relativ low at last no one spotted something and it is a world wide used thing at web scale.

# The core fundamentals of simplicity

## We should aim for simplicity because simplicity is a prerequisite for reliability.
This means if your software is not change able by a outside contributor in less then 1 day to fix his problems then your software is easy sayed not simple.

## Simple is often erroneously mistaken for easy. 
"Easy" means "to be at hand", "to be approachable". "Simple" is the opposite of "complex" which means "being intertwined", "being tied together". Simple != easy.

## What matters in software is: 
The answers to these questions is what matters in writing software not the look and feel of the experience writing the code or the cultural implications of it.
- does the software do what is supposed to do? 
- Is it of high quality? 
- Can we rely on it? 
- Can problems be fixed along the way? 
- Can requirements change over time? 

## The benefits of simplicity are: 
ease of understanding, ease of change, ease of debugging, flexibility, modules are pure functions that are recomposeable into a component. The mantra is alwas composition over inharitance. Never create a class or structure for data always view the data in your way.

## Complex constructs: 
State, Object, Methods, Syntax, Inheritance, Switch/matching, Vars, Imperative loops, Actors, ORM, Conditionals.

## Simple constructs: 
Const, Functions, Data, Polymorphism, Managed refs, Streams, Declarative data manipulation, Rules, Consistency.

## Build simple systems by: 
Abstracting - design by answering questions related to what, who, when, where, why, and how.
Choosing constructs that generate simple artifacts like modules that do not reference other modules without a unified resolver method that produces static in memory references...
Simplify by encapsulation via composition of functions and streams.


## Ok you understood it now!
Let me show you where clever systems in the world tryed to guide you into the right direction.

### Git
Many people know it and even more hate it. While when understood and applyed correct is the essence of simplicity it even has that in its name and it is all over. 
- It has the core concept of modules written as indipendent binarys. 
- It turns your string content so text into versioned hash referenced modules that are recompose able.

so you see git does much more then host content it turns your content into modules any text that you add via a commit gets its own module every commit is a own module. 

maybe that also helps you to identifie a good commit from a bad one. If a code commit that is not chor for the whole repo touches more then 1 Module or on higher level more then 1 component. Then you found bad code! That is the time where you need to take action and turn it back into a maintainable state.


