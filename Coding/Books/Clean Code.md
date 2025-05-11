## Amazon Link
[Clean Code: A Handbook of Agile Software Craftmanship by Robert C. Martin](https://www.amazon.com/Clean-Code-Handbook-Software-Craftsmanship/dp/0132350882)
## Referenced Books
- [Literate Programming by Donald E. Knuth](https://www-cs-faculty.stanford.edu/~knuth/lp.html)
- [Implementation Patterns by Kent Beck, Addison-Wesley](https://www.amazon.com/Implementation-Patterns-Kent-Beck/dp/0321413091)
# Notes
## Foreward
- The 5S Philosophy
	- *Seiri*, or organization (think "sort" in English). Knowing where things are and using approaches such as suitable naming is crucial
	- *Seiton*, or tidiness (think ""systematize" in English). There is an old American saying: *A place for everything, and everything in its place.* A piece of code should be where you expect to find it--and, if not,  you should re-factor to get it there
	- *Seiso*, or cleaning (think "shine" in English): Keep the workplace free of hanging wires, grease, scraps, and waste. What do the authors here say about lingering your code with comments and commented-out code lines that capture history or wishes for the future? Get rid of them
	- *Seiketsu*, or standardization: The group agrees about how to keep the workplace clean. Do you think this book says anything about having a consistent coding style and set of practices within the group? Where do those standards come from?
	- *Shutsuke*, or discipline (*self*-discipline). This means having the discipline to follow the practices and to frequently reflect on one's work and be willing to change

- Making code readable is as important as making it executable
## Chapter 1 - Clean Code
> I like my code to be elegant and efficient. The logic should be straightforward to make it hard for bugs to hide, the dependencies minimal to ease maintenance, error handling complete according to an articulated strategy, and performance close to optimal so as not to tempt people to make the code messy with unprincipled optimizations. Clean code does one thing well.
Bjarne Stroustrup, inventor of C++
- Bad code *tempts* the mess to grow
- Clean code exhibits close attention to detail
> Clean code is simple and direct. Clean code reads like well-written prose. Clean code never obscures the designer's intent but rather is full of crisp abstractions and straightforward lines of control.
Grady Booch
- Code should be matter-of-fact as opposed to speculative
> Clean code can be read, and enhanced by a developer other than its original author. It has unit and acceptance tests. It has meaningful names. It provides one way rather than many ways for doing one thing. It has minimal dependencies, which are explicitly defined, and provides a clear and minimal API. Code should be literate since depending on the language, not all necessary information can be expressed clearly in code alone.
"Big" Dave Thomas, founder of OTI
- Clean code makes it easy for *other* people to enhance it
- Code, without tests, is not clean

> I could list all of the qualities that I notice in clean code, but there is one overarching quality that leads to all of them. Clean code always looks like it was written by someone who cares. There is nothing obvious that you can do to make it better. All of those thing were thought about by the code's author, and if you try to imagine improvements, you're led back to where you are, sitting in appreciation of the code someone left for you --code left by someone who cares deeply about the craft.
Michael Feathers

> In recent years I begin, and nearly end, with Beck's rules of simple code: In priority order, simple code:
> - Runs all the tests;
> - Contains no duplication;
> - Expresses all the design ideas that are in the system;
> - Minimizes the number of entities such as classes, methods, functions, and the like;
Ron Jeffries

> You know you are working on clean code when each routine you read turns out to be pretty much what you expected. You can call it beautiful code when the code also makes it look like the language was made for the problem.
Ward Cunningham, inventor of Wiki

- If we all checked-in our code a little cleaner than when we checked it out, the code simply could not rot
## Chapter 2 - Meaningful Names
- Use intention-revealing names
	- Take care with your names and change them when you have better ones
	- The name of a variable, function, or class, should answer all the big questions. It should tell you why it exists, what it does, and how it is used. If a name requires a comment, then the name does not reveal its intent.
- Beware of using names which vary in small ways
- Programmers create problems for themselves when they write code solely to satisfy a compiler or interpreter
- My personal preference is that single-letter names can ONLY be used as local variables inside short methods
- *The length of a name should correspond to the size of its scope*
- If you must encode either the interface or the implementation, choose the implementation. Call it `ShapveFactoryImp` or even the hideous `CShapeFactory` is preferable to encoding the interface
- One difference between a smart programmer and a professional programmer is that the professional understands that *clarity is king*
### Naming
- Classes and objects should have noun or noun phrase names like `customer`, `WikiPage`, `Account`, and `AddressParser`. Avoid words like `Manager`, `Processor`, `Data`, or `Info` in the name of a class. A class name should not be a verb #classNaming
- Methods should have verb or verb phrase names like `postPayment`, `deletePage`, or `save`. Accessors, mutators, and predicates should be named for their value and prefixed with `get`, `set`, and `is` #methodNaming
- When constructors are overloaded, use static factory methods with names that describe the arguments. For example: `Complex fulcrumPoint = Complex.FromRealNumber(23.0);`
- Pick one word per concept
- Avoid using the same word for two purposes
- There are lots of very technical things that programmers have to do. Choosing technical names for those things is usually the most appropriate course.
	- When there is no "programmer-eese" for what you're doing, use the name from the problem domain
- There are a few names which are meaningful in and of themselves--most are not. Instead, you need to place names in context for your reader by enclosing them in well-named classes, functions, or namespaces. When all else fails, then prefixing the name may be necessary as a last resort
- Shorter names are generally better than longer ones, so long as they are clear
## Chapter 3 - Functions
- The first rule of functions is that they should be small
- Lines should not be 150 characters long. Functions should not be 100 lines long. Functions should hardly ever be 20 lines long
- The indent level of a function should not be greater than one or two
- Functions should do one thing. They should do it will. They should do it only
	- If a function does only those steps that are one level below the stated name of the function, then the function is doing one thing
	- Functions that do one thing cannot be reasonably divided into sections
- In order to make sure our functions are doing "one thing," we need to make sure that the statements within our function are all at the same level of abstraction
- We want the code to read like a top-down narrative. We want every function to be followed by those at the next level of abstraction so that we can read the program, descending on level of abstraction at a time as we read down the list of functions
	- We want to be able to read the program as though it were a set of TO paragraphs, each of which is describing the current level of abstraction and referencing subsequent TO paragraphs at the next level down
> 		To include the setups and teardowns, we include setups, then we include the test page content, and then we include the teardowns.
- It is hard to make a small `switch` statement. Even a `switch` statement with only two cases is larger than I'd like a single block or function to be. It is also hard to make a `switch` statement that does one thing. By their nature, `switch` statements always do N things. Unfortunately, we cannot always avoid `switch` statements, but we *can* make sure that each `switch` statement is buried in a low-level class and is never repeated. We do this, of course, with polymorphism.
	- Bury them in an ABSTRACT FACTORY and never let anyone see it. The factory will then use the `switch` statement to create appropriate instances of the derivatives
	- My general rule for `switch` statements is that they can be tolerated if they appear only once, are used to create polymorphic objects, and are hidden behind an inheritance relationship so that the rest of the system cannot see them
- The ideal number of arguments for a function is zero (niladic). Next comes one (monadic), followed closely by two (dyadic). Three arguments (triadic) should be avoided where possible. More than three (polyadic) requires very special justification--and then should not be used anyway
- There are two very common reasons to pass a single argument into a function. You may be asking a question about that argument, as in `boolean fileExists("My-File")` or you may be operating on that argument, transforming it into something else and *returning it*
	- A somewhat less common, but still very useful form for a single argument function, is an *event*. In this form there is an input argument but no output argument. The overall program is meant to interpret the function call as an event and use the argument to alter the state of the system
- Flag arguments are ugly. Passing a boolean into a function is a truly terrible practice. It immediately complicates the signature of the method, loudly proclaiming that this function does more than one thing. It does one thing if the flag is true, and another if the flag is false
- The second parameter in a dyadic function requires a short pause until we learn to ignore the first parameter. And *that*, of course, eventually results in problems because we should never ignore any port of code. The parts we ignore are where the bugs will hide
- When a function seems to need more than two or three arguments, it is likely that some of those arguments ought to be wrapped into a class of their own
- If the variable argumenets are all treated identically, then they are equivalent to a single argument of type list (i.e. `public String format(String format, Object...args)`
- Encode the names of the arguments into the function name. For example, `assertEquals` might be better written as `assertExpectedEqualsActual`. This strongly mitigates the problem of having to remember the ordering of the arguments
- Side effects are lies. Your function promises to do one thing, but also does other hidden things
- In general output arguments should be avoided. If your function must change the state of something, have it change the state of its owning object
- Functions should either do something or answer something, but not both
- Prefer exceptions to returning code errors
- `try/catch` blocks are ugly in their own right. They confuse the structure of the code and mix error processing with normal processing. So it is better to extract the bodies of the `try` and `catch` blocks out into functions of their own
	- Functions should do one thing. Error handling is one thing
- Writing software is like any other kind of writing. When you write a paper or an article, you get your thoughts down first, then you massage it until it reads well. The first draft might be clumsy and disorganized, so you wordsmith it and restructure it and refine it until it reads the way you want it to read
- Functions are the verbs of programming languages, and classes are the nouns
## Chapter 4 - Comments
- The proper use of comments is to compensate for our failure to express ourself in code
## Chapter 5 - Formatting
- Small files are usually easier to understand than large files
- Blank lines that separate the package declaration, the import(s), and each of the functions. This extremely simple rule has a profound effect on the visual layout of the code. Each blank line is a visual cue that identifies a new a separate concept
- Variables should be declared as close to their usage as possible. Because our functions are very short, local variables should appear at the top of each function
	- In rare cases a variable might be declared at the top of a block or just before a loop in a long-ish function
- **Instance variables**, on the other hand, should be declared at the top of the class
- If one function calls another, they should be vertically close, and the caller should be above the callee, if at all possible
- The old Hollerith limit of 80 is a bit arbitrary, and I'm not opposed to lines edging out to 100 or even 120. But beyond that is probably just careless
## Chapter 6 - Objects and Data Structures
- We do not want to expose the details of our data. Rather we want to express our data in abstract terms
- Objects hide their data behind abstractions and expose functions that operate on that data. Data structures expose their data and have no meaningful functions
- Procedural code (code using data structures) makes it easy to add new functions without changing the existing data structure. OO code, on the other hand, makes it easy to add. new classes without changing existing functions
	- Vice versa - Procedural code makes it hard to add new data structures because all the functions must change. OO code makes it hard to add new functions because all the classes must change
- Hybrids (half object and half data structure) - Have functions that do significant things, and they also have either public variables or public accessors and mutators that, for all intents and purposes, make the private variables public, tempting other external functions to use those variables the way a procedural program would use a data structure. 
	- Such hybrids make it hard to add new functions, but also make it hard to add new data structures. They are the worst of both worlds. Avoid creating them
- The quintessential form of a data structure is a class with public variables and no functions. This is sometimes called a data transfer object (DTO). DTOs are very useful structures, especially when communicating with databases or parsing messages from sockets, and so on. They often become the first in a series of translation stages that convert raw data in a database into objects in the application code.
- Active Records are special forms of DTOs. They are data structures with public (or bean-accessed) variables; but they typically have navigational methods like `save` and `find`. Typically these Active Records are direct translations from database tables, or other data sources
## Chapter 7 - Error Handling
- It is a good practice to start with a `try-catch-finally` statement when you are writing code that could throw exceptions. This helps you define what the user of that code should expect, no matter what goes wrong with the code that is executed in the `try`
- Checked exceptions can sometimes be useful if you are writing a critical library: You must catch them. But in general application development the dependency costs outweigh the benefits
- Create informative error messages and pass them along with your exceptions. Mention the operation that failed and the type of failure. If you are logging in your application, pass along enough information to be able to log the error in your `catch`
- When we define exception classes in an application, our most important concern should be `how they are caught`
- Wrapping third-party APIs is a #bestPractice. When you wrap a third-party API, you minimize your dependencies upon it: You can choose to move to a different library in the future without too much penalty. Wrapping also makes it easier to mock out third-party calls when you are testing your own code
- The SPECIAL CASE PATTERN [Fowler]. You create a class or configure an object so that it handles a special case for you. When you do, the client code does not have to deal with exceptional behavior. That behavior is encapsulated in the special case object.
- If you are tempted to return `null` from a method, consider throwing an exception or returning a SPECIAL CASE object instead. If you are calling a `null`-returning method from a third-party API, consider wrapping that method with a method that either throws an exception or returns a special case object
## Chapter 8 - Boundaries
- If you use a boundary interface like `Map`, keep it inside the class, or close family of classes, where it is used. Avoid returning it from, or accepting it as an argument to public APIs
- Learning the third-party code is hard. Integrating the third-party code is hard too. Doing both at the same time is doubly hard. What if we took a different approach? Instead of experimenting and trying out the new stuff in your production code, we could write some tests to explore our understanding of the third-party code. Jim Newkirk calls such tests *learning tests*
- The ADAPTER encapsulates the interaction with the API and provides a single place to change when the API evolves #bestPractice 
- We manage third-party boundaries by having very few places in the code that refer to them. We may wrap them as we did with `Map`, or we may use an ADAPTER to convert from our perfect interface to the provided interface
## Chapter 9 - Unit Tests
- **First Law** - You may not write production code until you have written a failing unit test
- **Second Law** - You may not write more of a unit test than is sufficient to fail, and not compiling is failing
- **Third Law** - You may not write more production code than is sufficient to pass the currently failing test
- Test code is just as important as production code
- Readability is perhaps even more important in unit tests than it is in production code. What makes tests readable? The same thing that makes all code readable: clarity, simplicity, and density of expression. In a test you want to say a lot with as few expressions as possible
- The BUILD-OPERATE-CHECK pattern
	- The first part build up the test data
	- The second part operates on that test data
	- The third part checks that the operation yielded the expected results
- Building a domain-specific language for your tests - Rather than using the APIs that programmers use to manipulate the system, we build up a set of functions and utilities that make use of those APIs and that make the tests more convenient to write and easier to read
- The single assert rule is a good guideline. I usually try to create a domain-specific testing language that supports it #bestPractice
- F.I.R.S.T
	- Fast - Tests should be fast
	- Independent - Tests should not depend on each other
	- Repeatable - Tests should be repeatable in any environment
	- Self-Validating - Tests should have a boolean output
	- Timely - The tests need to be written in a timely fashion. Unit tests should be written *just before* the production code that makes them pass
## Chapter 10 - Classes
- A class should begin with a list of variables. Public static constants, if any, should come first. Then private static variables, followed by private instance variables. There is seldom a good reason to have a public variable
- Public functions should follow the list of variables. We like to put the private utilities called by a public function right after the public function itself
- The first rule of classes is that they should be small
- With classes we measure size by responsibilities
- We should also be able to write a brief description of the class in about 25 words, without using the words "if," "and," "or," or "but."
- Classes should have a small number of instance variables. Each of the methods of a class should manipulate one or more of those variables. In general the more variables a method manipulates the more cohesive that method is to its class
- When classes lose cohesion, split them
- The Open-Closed Principle (OCP) - Classes should be open for extension but closed for modification
- The Dependency Inversion Principle (DIP) - Our classes should depend upon abstractions, not on concrete details
## Chapter 11 - Systems
- Software systems should separate the startup process, when the application objects are constructed and the dependencies are "wired" together, from the runtime logic that takes over after startup
- Software systems are unique compared to physical systems. Their architecture can grow incrementally, if we maintain the proper separation of concerns