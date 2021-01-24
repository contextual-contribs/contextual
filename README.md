# warning
If you love semicolons and lots of typing, you'll hate this language. 

If you want to type as little as possible, write code that's clean, understandable, and radically minimal, and to let the computer to figure what you mean, read on. 

# contextual
What if you could invent a new programming language, designed purely to simplify your life as a programmer, without *any* of the constraints of existing languages? 

This is a proposal for a new programming language, or meta-language, designed for radical brevity plus human-readability. Think CoffeScript or Clojure without all the cruft. 

This project is bold enough to propose coding practice which some people might find scary. The radical goals of this project will not be comfortable for everyone, and we're OK with that. We're not trying to please everyone. We're trying to please programmers who are tired of having to over-explain themselves to the computer. 

# why javascript?
contextual is planned a a javascript transpiler. Why javascript? Because we hate javascript, but it's ubiquitous. We're tired of the timid evolution of javascript. 

We hope contextual.js will inspire other radically-sparse languages. 


# example
Which one do YOU find easier to read? Be honest. 

**Javascript**

105 chars

(each indent counts as one char)
```
greetByName('Jack')

function greetByName(sName) {
    if (!sName) {
        console.log ('Hi');
        }
    else {
        console.log ('Hello, ' + sName);
        };
    };
```

**contextual, proposed:** 

36 chars
````
greetByName'Jack'

greetByName
    ! Say
        'Hello ' sName
        'Hi'    
````
The contextual version has strong typing and locally-scoped variables. 

[Full explanation](https://github.com/contextual-contribs/contextual/wiki/Snip:-Function-With-Conditional)


# philosophy
The core philosophies of this meta-language are:
- Eliminate "machinery" in code. That is, most (all?) code today is packed with instructions to the parser[1], which aren't necessarily useful to the programmer, and often reduce readability. For example, punctuation. 
- Make the parser smarter. Exploit parser-intelligence to radically reduce programmer effort. 
- Eliminate the obvious. Depend on context and implication. Enable the parser to make assumptions based on context. 
- Use the sparsest means to eliminate contextual redundancy (preferably whitespace or single characters)
- Eliminate redundancy. 
- Eliminate variables whenever possible. 
- Favor the most common patterns. Use the most minimal syntax for common patterns, with optional syntax for uncommon patterns. Make the most common coding patterns part of the language, so the programmer doesn't have to spell them out every time. 
- Enable programmer to customize language-keywords. 
- Strongly-typed.

[1]: (Using the word "parser" to refer to IDE, linters, parsers, transpilers, and compilers. Anything that interprets the code.)


# design
- Use symbols in place of verbose coding structures. 
- Use defaults to eliminate typing of the obvious. 
- Imply structure with whitespace and positioning. 
- Imply parameters and variables. 
- Strongly type variables by usage. 


# goals
1. Define the language. Resolve all ambiguities. 
2. Build a Javascript transpiler. 


# progress
Current phase is **brainstorming phase.** The only activity right now is for the community to dream up better, briefer ways to write code. No work will be done on a parser, transpiler, or compiler at this time. 
