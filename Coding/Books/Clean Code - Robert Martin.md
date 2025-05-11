### Foreward
- "You should name a variable using the same care with which you name a first-born child."
- "We abandon our code early, not because it is done, but because our value system focuses more on outward appearance than on the substance of what we deliver."
### Introduction
- The only valid measurement of code quality is how easy it is to read.

### Chapter 1 - Clean Code
- Bad code leads to lower productivity (slower bug fixes, new feature releases).. "As productivity decreases, management does the only thing they can; they add more staff to the project in hopes of increasing productivity. But that new staff is not versed in the design of the system."
- "Clean code does one thing well"
- Bad code tries to do too much, it has muddled intent and ambiguity of purpose. Clean code is focused.
- "When the same thing is done over and over, it's a a sign that there is an idea in our mind that is not well represented in the code."
- "I also look at whether an object or method is doing more than one thing. If it's an object, it probably needs to be broken into two or more objects. If it's a method, I will always use the Extract Method refactoring (pulls logic into a new sub method) on it , resulting in one method that says clearly what it does, and some sub-methods saying how it is done." <- **Can be used to improve dirty code**
- "... we often find ourselves wanting a particular item from that collection. When I find that happening, I will often wrap the particular implementation in a more abstract method or class **(i.e. helper classes or an abstract base class that the processing class can inherit from)**. That gives me a couple of interesting advantages.
	- I can implement the functionality now with something simple, say a hash map, but since now all references to that search are covered by my little abstraction, I can change the implementation any time I want. I can go forward quickly while preserving my ability to change later.
	- In addition, the collection abstraction often cals my attention to what's 'really' going on, and keeps me from running down the path of implementing arbitrary collection behavior when all I really need is a few fairly simple ways of finding what I want."
- "Reduced duplication, high expressiveness, and early building of simple abstractions. That's what makes clean code for me."
- No duplication, one thing, expressiveness, tiny abstractions.
- "You know you are working on clean code when each routine you read turns out to be pretty much what you expected. You can call it beautiful code when the code also makes it look like the language was made for the problem"
- It is not the language that makes programs appear simple. It is the programmer that makes the language appear simple!
### Chapter 2 - Meaningful Names
- The length of a name should correspond to the size of its scope. <- The more a variable is used the more detailed the name should be (to make it easier to read and search).
- One difference between a smart programmer and an professional programmer is the professional understands that clarity is king.
- Classes and objects should have noun or noun phrase names.
- Methods should have verb of verb phrase names.
- Accessors, mutators, and predicates should be named for their value and prefixed with `get`, `set`, and `is` (consider enforcing their use by making the corresponding constructors private)
- Pick one word per abstract concept and stick with it.
- Avoid using the same word for two purposes.
	- Ex: add for creating a new value by concatenating to a string vs. appending to a list.
- Shorter names are generally better than longer ones, so long as they are clear.
- 