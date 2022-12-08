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

How does maintainable state look like?
you need indipeendent working code and a unified reference to it most best this reference includes a content hash to verifie the content it self which is the code. When you want something more dynamic then a content hash you could also simply add a verification module after loading the module the verification needs not to depend on a hash it can depend on it.

in general you need something that is called a identity provider or access manager for your modules. Something that routes capabilitys to the modular code. So you can be save that it only does what it should do and nothing else.

git again provides that via its commit messages it is the verification protocol for the modules. while this messages often get abused for all kind of other stuff they are mainly designed only for verification of the module it self they contain the code changes in a readable so simple way to think about them. 

### Object Based Databases Document based and other buzzwords
All products in the familiy of Databases that are Object Document Based do inhirently embrace the concepts of simplicity. Every single documentation about the database design is in general documentation about how to design simple systems. Thats also the reason why most developers choose to even use a database as the backend it makes thinking for them more simple

while databases it self are a historical thing they existed to solve the so called cache problems of slow hardisks when random accessed. They did so via a index the cache that could be queried to directly know without additional lookup where the data is. So it reduced the roundtrips. Thats why they existed. But today they are still all over the question is why?

The answer is beecause developer knowlege is decreasing with the decades as the amount of developers doubles to fast we always got over 50% of developers with less expirence then 5 years and also in that 5 years they often do not get teached by persons who do real code work. 

## The question about the language of the future?
There is not a real question there exist only 2 languages ECMAScript and ASM ok i know that is shoking now but that is what it is. ECMAscript got most best implemented via the v8 engine today which is written in C++ that is a nice hybrid syntax that makes c more simple which then at the end will get translated to ASM or instructions that can get translated to ASM. That depends on if it is usefull to finaly compile the code for the target or better compile it on the target it self. 

The future of V8 how ever is ECMAScript it self generating ASM. In fact that is already WiP via a tiny project that is called JustJS. It is a a Prototype and also the proof that it is possible and the right thing to do. The man who created and published that example is in my view a legend even if he does maybe or maybe not understand what he did there. I never had time to talk much with him about none tech details and still i feel connected because he intentional shows me with his code that he understands the concepts of simplicity and he does execute them. I do not even know what drives him but as i saw it i was 100% sure that it is time to publish that. I my self was to deep into other research to come up with such a complet well done solution like he did. 

## Inspiring Examples that i did create to challenge your mind

#### Compile a ECMAScript Module out of a git file reference 
remember the fundamentals Build simple systems by: 
Abstracting - design by answering questions related to what, who, when, where, why, and how.
Choosing constructs that generate simple artifacts like modules that do not reference other modules without a unified resolver method that produces static in memory references...
Simplify by encapsulation via composition of functions and streams.

```js
// what? Compile a ECMAScript Module out of a git file reference
// who? import('git-client')
// when? as soon as ready we use the functional stream pattern.
// where? inMemory 
// why? because we want to instantiate it to do something with it
// how? simply read the above questions and then you will already know the solution the concept of simple self explaining code.
```


take all commits exempt a single one aka cherry picking commits based on a file that referencs the last commit that modified it in the current git repo branch. 

```js
/// .....
```

test.module-v1.0.0-beta.0.js
```js
export const moduleMethodName = () => { /** this is a NoOp no operationg */ };
```
