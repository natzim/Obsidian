## Amazon Link
- [The Pragmatic Programmer: From Journeyman to Master](https://www.amazon.com/Pragmatic-Programmer-Journeyman-Master/dp/020161622X)
## Referenced Books
- [Mythical Man-Month, The: Essays on Software Engineering](https://www.amazon.com/Mythical-Man-Month-Software-Engineering-Anniversary/dp/0201835959)
- [Peopleware: Productive Projects and Teams](https://www.amazon.com/Peopleware-Productive-Projects-Tom-DeMarco/dp/0932633439)
- [Dinosaur Brains: Dealing with All Those Impossible People at Work](https://www.amazon.com/Dinosaur-Brains-Dealing-Impossible-People/dp/0345410211)
- [Refactoring: Improving the Design of Existing Code]()
# Notes
## Chapter 1 - A Pragmatic Philosophy
 - What distinguishes Pragmatic Programmers? We feel it’s an attitude, a style, a philosophy of approaching problems and their solutions. They think beyond the immediate problem, placing it in its larger context and seeking out the bigger picture.
### Topic 1 - It's Your life
### Topic 2 - The Cat Ate My Source Code
- Pragmatic Programmers take charge of their own career, and aren't afraid to admit ignorance or error.
- Above all, your team needs to be able to trust and rely on you-and you need to be comfortable relying on each of them as well. Trust in a team is absolutely essential for creativity and collaboration according to the [research literature](http://dx.doi.org/10.1037/apl0000110).
- Before you approach anyone to tell them why something can't be done, is late, or is broken, stop and listen to yourself
- When you find yourself saying, 'I don’t know,' be sure to follow it up with '—but I’ll find out.' It’s a great way to admit what you don’t know, but then take responsibility like a pro.
### Topic 3 - Software Entropy
- Don’t leave 'broken windows' (bad designs, wrong decisions, or poor code) unrepaired. Fix each one as soon as it is discovered. If there is insufficient time to fix it properly, then board it up. Perhaps you can comment out the offending code, or display a 'Not Implemented' message, or substitute dummy data instead. Take some action to prevent further damage and to show that you’re on top of the situation.
- Don’t cause collateral damage just because there’s a crisis of some sort. One broken window is one too many.
### Topic 4 - Stone Soup and Boiled Frogs
- You may be in a situation where you know exactly what needs doing and how to do it. The entire system just appears before your eyes—you know it’s right. But ask permission to tackle the whole thing and you’ll be met with delays and blank stares. People will form committees, budgets will need approval, and things will get complicated. Everyone will guard their own resources. Sometimes this is called “start-up fatigue.’’ It’s time to bring out the stones. Work out what you can reasonably ask for. Develop it well. Once you’ve got it, show people, and let them marvel. Then say "of course, it would be better if we added…" Pretend it’s not important. Sit back and wait for them to start asking you to add the functionality you originally wanted. People find it easier to join an ongoing success. Show them a glimpse of the future and you’ll get them to rally around.
- Constantly review what's happening around you, not just what you personally are doing.
### Topic 5 - Good-Enough Software
- You can discipline yourself to write software that's good enough for your users for future maintainers, for your own peace of mind. You'll find that you are more productive and your users are happier. And you may well find that your programs are actually better for their short incubation
- Many users would rather use software with some rough edges *today* than wait a year for the shiny, bells-and-whistles version.
- Don't spoil a perfectly good program by over-embellishment and over-refinement
### Topic 6 - Your Knowledge Portfolio
- To be successful in your career, you must invest in your knowledge portfolio using the same guidelines [as investors] (1. Invest regularly. 2. Diversify. 3. Balance portfolios. 4. By low and sell high. 5. Reviewed and rebalanced regularly). The good news is that managing this kind of investment is a skill just like any other-it can be learned. The trick is to make yourself do it initially and for a habit. Develop a routine which you follow unit
	- Invest Regularly - In your knowledge portfolio. Find a consistent time and place away from interruptions.
	- Diversify - The more different things you know, the more valuable you are. Know the technologies you are working with, keep up with changes and add other skills even in non-technical areas like communication
	- Manage Risk - Don't put all your technical eggs in one basket
	- Buy Low, Sell High - Learn emerging technologies before it becomes popular
	- Review and Rebalance - New technologies are always emerging. Invest in learning them. Put time into learning new languages
- Goals
	- Learn at least one new language a year
		- Different languages solve the same problems in different ways which broadens your thinking
	- Read a technical book each month
	- Read nontechnical books too
	- Experiment with different environments
	- Stay current
- So you’re reading voraciously, you’re on top of all the latest breaking developments in your field (not an easy thing to do), and somebody asks you a question. You don’t have the faintest idea what the answer is, and freely admit as much. Don’t let it stop there. Take it as a personal challenge to find the answer. Ask around. Search the web—the scholarly parts too, not just the consumer parts. If you can’t find the answer yourself, find out who can. Don’t let it rest. Talking to other people will help build your personal network, and you may surprise yourself by finding solutions to other, unrelated problems along the way. And that old portfolio just keeps getting bigger….
- Beware of the zealots who insist that their dogma provides the only answer.
- Critical thinking is an entire discipline unto itself, and we encourage you to read and study all you can about it
	- Ask the "Five Whys"
	- Who does this benefit?
	- What's the context?
		- Consider an article or book touting a 'best practice.' Good questions to consider are 'best for who?' What are the prerequisites, what are the consequences, short and long term...
	- When or Where would this work?
	- Why is this a problem?
### Topic 7 - Communicate!
- Treat English as just another programming language
- You're communicating only if you're conveying what you mean to convey-just talking isn't enough. To do that, you need to understand the needs, interests, and capabilities of your audience.
- Plan what you want to say. Write an outline. Then ask yourself, "Does this communicate what I want to express to my audience in a way that works for them?" Refine it until it does.
- Make what you're saying relevant in time, as well as in context.
- Keeping people informed makes them far more forgiving of the occasional slip, and makes them feel that you haven't forgotten them.
- Finally, there’s the matter of communicating via documentation. Typically, developers don’t give much thought to documentation. At best it is an unfortunate necessity; at worst it is treated as a low-priority task in the hope that management will forget about it at the end of the project. Pragmatic Programmers embrace documentation as an integral part of the overall development process. Writing documentation can be made easier by not duplicating effort or wasting time, and by keeping documentation close at hand—in the code itself. In fact, we want to apply all of our pragmatic principles to documentation as well as to code.
- Commenting source code gives you the perfect opportunity to document those elusive bits of a project that can’t be documented anywhere else: engineering trade-offs, why decisions were made, what other alternatives were discarded, and so on.
- Challenges
	- There are several good books that contain sections on communications within teams, including The Mythical Man-Month: Essays on Software Engineering and Peopleware: Productive Projects and Teams. Make it a point to try to read these over the next 18 months. In addition, Dinosaur Brains: Dealing with All Those Impossible People at Work  discusses the emotional baggage we all bring to the work environment. #book
## Chapter 2 - A Pragmatic Approach
### Topic 8 - The Essence of Good Design
- ETC - Easier to Change
	- Good design is easier to change than bad design
- Try to make what you write replaceable. That way, whatever happens in the future, this chunk of code won't be a roadblock.
### Topic 9 - DRY - The Evils of Duplication
- DRY - Don't repeat yourself
- Every piece of knowledge must have a single, unambiguous, authoritative representation within a system.
- DRY is about the duplication of *knowledge*, of *intent*. It's about expressing the same thing in two different places, possibly in two totally different ways.
- All services offered by a module should be available through a uniform notation, which does not betray whether they are implemented through storage or through computation
- Not all code duplication is knowledge duplication. I.E. two different concepts may coincidentally have overlapping logic. If it's two separate concepts, it is not duplicate code to have the logic written in two separate places.
- Increasingly, you'll find that public APIs are documented formally using something like OpenAPI. This allows you to import the API spec into your local API tools and integrate them more reliably with the service.
- There’s another option, and one we often prefer. Rather than writing code that represents external data in a fixed structure (an instance of a struct or class, for example), just stick it into a key/value data structure (your language might call it a map, hash, dictionary, or even object). On its own this is risky: you lose a lot of the security of knowing just what data you’re working with. So we recommend adding a second layer to this solution: a simple table-driven validation suite that verifies that the map you’ve created contains at least the data you need, in the format you need it. Your API documentation tool might be able to generate this.
### Topic 10 - Orthogonality
- Two or more things are orthogonal if changes in one do not affect any of the others.
- When components of any system are highly interdependent, there is no such thing as a local fix. 
- Every time you write code you run the risk of reducing the orthogonality of your application. Unless you constantly monitor not just what you are doing but also the larger context of the application, you might unintentionally duplicate functionality in some other module, or express existing knowledge twice. 
	- To help prevent this: Keep your code decoupled, avoid global data, and avoid similar functions
- Get into the habit of being constantly critical of your code. Look for any opportunities to reorganize it to improve its structure and orthogonality.
### Topic 11 - Reversibility
- The mistake lies in assuming that any decision is cast in stone-and in not preparing for the contingencies that might arise. Instead of carving decisions in stone, think of them more as being written in the sand at the beach. A big wave can come along and wipe them out at any time.
### Topic 12 - Tracer Bullets
- Look for the important requirements, the ones that define the system. Look for the areas where you have doubts, and where you see the biggest risks. Then prioritize your development so that these are the first areas you code.
- Making a skeleton with minimal end-to-end functionality (not mocking like a prototype) will act like a tracer bullet. Proving that the project can be done and connecting all the layers together. It also has the following benefits:
	- Users get to see something working early
	- Developers build a structure to work in
	- You have in integration platform
	- You have something to demonstrate
	- You have a better feel for your progress
- The most daunting piece of paper is the one with nothing written on it. If you have worked out all the end-to-end interactions of your application, and have embodied them in code, then your team won't need to pull as much out of thin air. This makes everyone more productive, and encourages consistency.
### Topic 13 - Prototypes and Post-It Notes
- What sorts of things might you choose to investigate with a prototype? Anything that carries risk. Anything that hasn’t been tried before, or that is absolutely critical to the final system. Anything unproven, experimental, or doubtful. Anything you aren’t comfortable with.
### Topic 14 - Domain Languages
- Program close to the problem domain
	- Include the vocabulary, syntax, and semantics-the language-of the domain.
- RSpec and the Phoenix router are written in their host languages (Ruby and Elixir). They employ some fairly devious code, including metaprogramming and macros, but ultimately they are compiled and run as regular code. Cucumber tests and Ansible configurations are written in their own languages. A Cucumber test is converted into code to be run or into a datastructure, whereas Ansible specs are always converted into a data structure that is run by Ansible itself. As a result, RSpec and the router code are embedded into the code you run: they are true extensions to your code’s vocabulary. Cucumber and Ansible are read by code and converted into some form the code can use. We call RSpec and the router examples of internal domain languages, while Cucumber and Ansible use external languages.
- The downside of internal domain languages is that you’re bound by the syntax and semantics of that language. Although some languages are remarkably flexible in this regards, you’re still forced to compromise between the language you want and the language you can implement. Ultimately, whatever you come up with must still be valid syntax in your target language. Languages with macros (such as Elixir, Clojure, and Crystal) gives you a little more flexibility, but ultimately syntax is syntax. External languages have no such restrictions. As long as you can write a parser for the language, you’re good to go. Sometimes you can use someone else’s parser (as Ansible did by using YAML), but then you’re back to making a compromise. Writing a parser probably means adding new libraries and possibly tools to your application. And writing a good parser is not a trivial job. But, if you’re feeling stout of heart, you could look at parser generators such as bison or ANTLR, and parsing frameworks such as the many PEG parsers out there. Our suggestion is fairly simple: don’t spend more effort than you save. Writing a domain language adds some cost to your project, and you’ll need to be convinced that there are offsetting savings (potentially in the long term). In general, use off-the-shelf external languages (such as YAML, JSON, or CSV) if you can. If not, look at internal languages. We’d recommend using external languages only in cases where your language will be written by the users of your application.
### Topic 15 - Estimating
- Estimate to avoid surprises
- Use units to give proper expectations

| Duration   | Quote estimate in                    |
| ---------- | ------------------------------------ |
| 1-15 days  | Days                                 |
| 3-6 weeks  | Weeks                                |
| 8-20 weeks | Months                               |
| 20+ weeks  | Think hard before giving an estimate |
- A basic estimating trick that always gives good answers: ask someone who's already done it
- You need to make it a habit to think about the scope before starting to guess.
- Building an estimation
	- Understand what's being asked - Build a rough-and-ready bare-bones mental model for the estimation
	- Build a model of the system - Building the model introduces inaccuracies into the estimating process. This is inevitable, and also beneficial. You are trading off model simplicity for accuracy. Doubling the effort on the model may give you only a slight increase in accuracy. Your experience will tell you when to stop refining.
	- Break the model into components - Break the model into components. 
	- Give each parameter a value
	- Calculate the answers
	- Keep track of your estimating prowess - Keep a record of how close you were. It will help calibrate
- Estimating project schedules
	- Give a range based on varying factors.
		- U.S. Navy uses PERT - Program Evaluation Review Technique which includes optimistic, most likely, and pessimistic estimates.
	- Give estimations based on iterations
## Chapter 3 - The Basic Tools
- Tools amplify talent
- Let need drive [tool] aquisitions
### Topic 16 - The Power of Plain Text
- Keep knowledge in plain text
- Plain text doesn't mean that the text is unstructured; HTML, JSON, YAML, and so on are all plain text
- Virtually every tool in the computing universe, from version control systems to editors to command-line tools, can operate on plain text
### Topic 17 - Shell Games
 - Gain familiarity with the shell, and you'll find your productivity soaring
### Topic 18 - Power Editing
### Topic 19 - Version Control
### Topic 20 - Debugging
- Embrace the fact that debugging is just *problem solving*, and attack it as such
- [create a] Failing test before fixing code
- When you're facing a massive stacktrace and you're trying to find out exactly which function mangled the value in error, you do a chop by choosing a stack frame somewhere in the middle and seeing if the error is manifest there. If it is, then you know to focus on the frames before, otherwise the problem is in the frames after. Chop again. Even if you have 64 frames in the stacktrace, this approach will give you an answer after at most six attempts.
- A very simple but particularly useful technique for finding the cause of a problem is simply to explain it to someone else (rubber ducking)
- Don't gloss over a routine or piece of code involved in the bug because you "know" it works. Prove it. Prove it in *this* context, with *this* data, with *these* boundary conditions
- When you come across a surprise bug, beyond merely fixing it, you need to determine why this failure wasn't caught earlier. Consider whether you need to amend the unit or other tests so that they would've caught it
- Debugging Checklist
	- Is the problem being reported a direct result of an underlying bug, or merely a symptom?
	- Is the bug *really* in the framework you're using? Is it in the OS?  Or is it in the code?
	- If you explain this problem in detail to a coworker, what would you say?
	- If the suspect code passes its unit tests, are the tests complete enough? What happens if you run the tests with *this* data?
	- Do the conditions that caused this bug exist anywhere else in the system? Are there other bugs still in the larval stage, just waiting to hatch?
### Topic 21 - Text Manipulation
- There are a number of great text manipulation languages. Unix developers often like to use the power of their command shells, augmented with tools such as `awk` and `sed`. People who prefer a more structured tool may prefer languages such as `Python` or `Ruby`.
### Topic 22 - Engineering Daybooks
- Try keeping an engineering daybook. Use paper, not a file or a wiki: there's something special about the act of writing compared to typing. Give it a month, and see if you're getting any benefits
- Daybooks are used to:
	- Jot down what we're working on
	- Note variable values when debugging
	- Leave reminders where to put things
	- Record wild ideas
	- ...
- Key benefits:
	- More reliable than memory
	- A place to store ideas that aren't immediately relevant
	- Acts as a kind of rubber duck
## Chapter 4 - Pragmatic Paranoia
- *They don't trust themselves, either*
### Topic 23 - Design by Contract
- Bertrand Meyer (Object-Oriented Software Construction) developed the concept of *Design by Contract* for the language Eiffel. It is a simple yet powerful technique that focuses on documenting (and agreeing to) the rights and responsibilities of software modules to ensure program correctness. What is a correct program? One that does no more and no less than it claims to do. Documenting and verifying that claim is the heart of *Design by Contract*  (DBC)
- Preconditions
	- What must be true in order fro the routine to be called; the routine's requirements. A routine should never get called when its preconditions would be violated. It is the caller's responsibility to pass good data.
- Postconditions
	- What the routine is guaranteed to do; the state of the world when the routine is done. The fact that the routine has a postcondition implies that it *will* conclude: infinite loops aren't allowed.
- Class Invariants
	- A class ensures that this condition is always true from the perspective of a caller. During internal processing of a routine, the invariant may not hold, but by the time the routine exits and control returns to the caller, the invariant must be true.
	- Note that a class cannot give unrestricted write-access to any data member that participates in the invariant.
	- If all the routine's preconditions are met by the caller, the routine shall guarantee that all postconditions and invariants will be true when it completes.
- Be strict in what you will accept before you begin, and promise as little as possible in return
- You can use *semantic invariants* to express inviolate requirements, a kind of "philosophical contract"
	- At Amazon these would be tenets
- Be sure not to confuse requirements that are fixed, inviolate laws with those that are merely policies that might change with a new management regime. That's why we use the term *semantic* invariants - it must be central to the very *meaning* of a thing, and not subject to the whims of policy (which is what more dynamic business rules are for)
### Topic 24 - Dead Programs Tell No Lies
- All errors give you information. You could convince yourself that the error can't happen, and choose to ignore it. Instead, Pragmatic Programmers tell themselves that if there is an error, something very, very bad has happened
- Some developers feel that it is good style to catch or rescue all exceptions, re-raising them after writing some kind of message. Their code is full of things like the code below.
	- Here's how Pragmatic Programmers would write this: `add_score_to_board(score);` We prefer it for two reasons. First, the application code isn't eclipsed by the error handling. Second, and perhaps more important, the code is less coupled.
```
try do
	add_score_to_board(score);
rescue InvalidScore
	Logger.error("Can't add invalid score. Exiting");
	raise
rescue BoardServerDown
	Logger.error("Can't add score: board is down. Exiting");
	raise
rescue StaleTransaction
	Logger.error("Can't add score: stale transaction. Exiting");
	raise
end
```
- "Defensive programming is a waste of time. Let it crash!" (Programming Erlang: Software for a Concurrent World by Joe Armstrong) In these environments, programs are designed to fail, but that failure is  managed with *supervisors*. A supervisor is responsible for running code and knows what to do in case the code fails, which could include cleaning up after it, restarting tit, and so on. What happens when the supervisor itself fails? Its own supervisor manages that event, leading to a design composed of *supervisor trees*. The technique is very effective and helps to account for the use of these languages in high-availability, fault-tolerant systems.
### Topic 25 - Assertive Programming
- Whenever you find yourself thinking "but of course that could never happen," add code to check it. The easiest way to do this is with assertions. In many language implementations, you'll find some form of `assert` that checks a Boolean condition. These checks can be invaluable
- Don't use assertions in place of real error handling. Assertions check for things that should never happen
### Topic 26 - How to Balance Resources
- Finish what you start
	- It simply means that the function or object that allocates a resource should be responsible for deallocating it
- When in doubt, it always pays to reduce scope
- Because Pragmatic Programmers trust no one, including ourselves, we feel that it is always a good idea to build code that actually checks that resources are indeed freed appropriately. For most applications, this normally means producing wrappers for each type or resource, and use these wrappers to keep track of all allocation and deallocations.
### Topic 27 - Don't Outrun Your Headlights
- Always take small, deliberate steps, checking for feedback and adjusting before proceeding. Consider that the rate of feedback is your speed limit. You never take on a step or a task that's "too big."
- What's a task that's too big? Any task that requires "fortune telling."
- Instead of wasting effort designing for an uncertain future, you can always fall back on designing your code to be replaceable
## Chapter 5 - Bend, or Break
### Topic 28 Decoupling
- When you're designing software you want it to be flexible, individual components should be coupled to as few other components as possible.
- Don't ask don't tell - This principle says that you shouldn't make decisions based on the internal state of an object and then update that object. Doing so totally destroys the benefit of encapsulation and, in doing so, spreads the knowledge of the implementation throughout the code
- The Law of Demeter
	- States that a method defined in a class `C` should only call:
		- Other instance methods in `C`
		- Its parameters
		- Methods in objects that it creates, both on the stack and in the heap
		- Global variables
	- In other words - Don't make chain method calls
		- Try not to have more than one "." when you access something. And *access something* also covers cases where you use intermediate variables
- Any mutable external resource is global data. If your application uses a database, datastore, file system, service API, and so on, it risks falling into the globalization trap. Again, the solution is to make sure you always wrap these resources behind code that you control
### Topic 29 - Juggling the Real World
- How to handle real life *events*
- Finite State Machines
	- Basically a specification on how to handle events
	- Can easily be expressed purely as data (such as a table with the current state and what to do)
	- Often underused by developers, but they don't solve all the problems associated with events
- Observer Pattern
	- Has source events called the observable and a list of clients called the observers
	- Particularly prevalent in user interface systems
	- The biggest problem is that because each observer has to register with the observable, it introduces coupling.
- Publish/Subscribe
	- Generalizes the observer pattern - Connects subscribers to publishers via *channels*
	- Good for decoupling the handling of async events
	- Does not handle creating systems that respond to a combination of events
- Reactive Programming and Streams
	- Streams let us treat events as if they were a collection of data. 
		- Allows us to treat streams just like any other collection
### Topic 30 - Transforming Programming
- All programs transform data, converting an input into an output
- Never pass raw values between transformations. Instead, wrap them in a data structure (or type) which also tells us if the contained value is valid. In Haskell, for example, this wrapper is called `Maybe`. In F# and Scala it's `Option`
- Thinking of code as a series of (nested) transformations can be a liberating approach to programming. It takes a while to get used to, but once you've developed the habit you'll find your code becomes much cleaner, your functions shorter, and your designs flatter.
### Topic 31 - Inheritance Tax
- Inheritance creates a lot of coupling
- Let us suggest three techniques that mean you should never need to use inheritance again:
	- Interfaces and protocols
		- Create no logic
		- Power because we can use them as types to any class implementing them will be compatible with that type
		- Prefer interfaces to express polymorphism
	- Delegation
		- With regular inheritance, if a parent class has 20 methods, and a subclass wants to make use of two of them, its objects will still have the other 18
		- Delegate to services: Has-A Trumps Is-A
	- Mixins and traits
		- Use Mixins to share functionality
### Topic 32 - Configuration
- Parameterize your app using external configuration
## Chapter 6 - Concurrency
### Topic 33 - Breaking Temporal Coupling
- On many projects, we need to model and analyze the application workflows as part of the design. We'd like to find out what *can* happen at the same time, and what *must* happen in a strict order. One way to do this is to capture the workflow using a notation such as the *activity diagram*
- You can use activity diagrams to maximize parallelism by identifying activities that *could be* performed in parallel, but aren't
- We're hoping to find activities that take time, but not in our code. Querying a database, accessing an external service, waiting for user input: all these things would normally stall our program until they complete. And these are all opportunities to do something more productive that the CPU equivalent of twiddling one's thumbs
### Topic 34 - Shared State is Incorrect State
- A semaphore is simply a *thing* that only one person can own at a time
- Random failures are often concurrency issues
### Topic 35 - Actors and Processes
- An *actor* is an independent virtual processor with its own local (and private) state. Each actor has a mailbox. When a message appears in the mailbox and the actor is idle, it kicks into life and processes the message. When it finishes processing, it processes another message in the mailbox, or, if the mailbox is empty, it goes back to sleep. When processing a message, an actor can create other actors, send messages to other actors that it knows about, and create a new state that will become the current state when the next message is processed
- A *process* is typically a more general-purpose virtual processor, often implemented by the operating system to facilitate concurrency. Processes can be constrained (by convention) to behave like actors, and that's the type of process we mean here
- In the actor model, there's no need to write any code to handle concurrency, as there is no shared state. There's also no need to code in explicit end-to-end "do this, do that" logic, as the actors work it out form themselves based on the messages they receive
### Topic 36 - Blackboards
- Some key features of the blackboard approach are:
	- None of the detectives need to know of the existence of any other detective - they watch the board for new information, and add their findings
	- The detectives may be trained in different disciplines, may have different levels of education and expertise, and may not even work in the same precinct. They share a desire to solve the case, but that's all
	- Different detectives may come and go during the course of the process, and may work different shifts
- Side-Note: Look into pre-tech processes for inspiration 
- This is a form of *laissez faire* concurrency. The detectives are independent processes, agents, actors, and so on. Some store facts on the blackboard. Others take facts off the board, maybe combining or processing them, and add more information to the board. Gradually the board helps them come to a conclusion.
## Chapter 7 - While You Are Coding
 - Conventional wisdom says that once a project is in the coding phase, the work is mostly mechanical. Transcribing the design into executable statements. We think that this attitude is the single biggest reason that software projects fail, and many systems end up ugly, inefficient, poorly structure, unmaintainable, or just plain wrong.
- Pragmatic Programmers think critically about all code, including our own
### Topic 37 - Listen to Your Lizard Brain
- When you feel a nagging doubt, or experience some reluctance when faced with a task, it might be that experience trying to speak to you. Heed it. You may not be able to put your finger on exactly what's wrong but give it time and your doubts will probably crystallize into something more solid, something you can address. Let your instincts contribute to your performance.
- Tell yourself you need to prototype something. If you're facing a blank screen, then look for some aspect of the project that you want to explore. Maybe you're using a new framework, and want to see how it does data binding. Or maybe it's a new algorithm, and you want to explore how it works on edge cases. Or maybe you want to try a couple different styles of user interaction
- If you're working on existing code and it's pushing back, then stash it away somewhere and prototype up something similar instead. Do the following:
	- Write "I'm prototyping" on a sticky note, and stick it on the side of your screen
	- Remind yourself that prototypes are meant to fail. And remind yourself that prototypes get thrown away, even if they don't fail. There is no downside to doing this.
	- In your empty editor buffer, create a comment describing in one sentence what you want to learn or do
	- Start coding
		- If you start to have doubts, look at the sticky note.
		- If, in the middle of coding, that nagging doubt suddenly crystallizes into a solid concern, then address it
		- If you get to the end of the experiment and you still feel uneasy, start again with the walk and the talk and the time off
- A large part of our job is dealing with existing code, often written by other people. Those people will have different instincts to you, and so the decisions they made will be different. Not necessarily worse; just different. 
	- You can read their code mechanically, slogging through it making notes on stuff that seems important. It's a chore, but it works.
	- Or you can try an experiment. When you spot things done in a way that seems strange, jot it down. Continue doing this, and look for patterns. If you can see what drove them to write code that way, you may find that the job of understanding it becomes a lot easier. You'll be able to consciously apply the patterns that they applied tacitly. And you might just learn something new along the way
- Learning to listen to your gut when coding is an important skill to foster. But it applies to the bigger picture as well. Sometimes a design just feels wrong, or some requirement makes you feel uneasy. Stop and analyze these feelings. If you're in a supportive environment express them out loud. Explore them. The chances are there's something lurking in that dark doorway. Listen to your instincts and avoid the problem before it jumps out at you.
### Topic 38 - Programming by Coincidence
- Don't assume it, prove it
- Finding an answer that happens to fit is not the same as the right answer
- We want to spend less time churning out code, catch and fix errors as early in the development cycle as possible, and create fewer errors to begin with. It helps if we can program deliberately:
	- Always be aware of what you are doing (don't be like a boiled frog)
	- Can you explain the code, in detail, to a more junior programmer?
	- Don't code in the dark, build an application you don't fully grasp, or use a technology you don't understand. If you do, you'll likely be bitten by coincidences. If you're not sure why it works, you won't know why it fails
	- Rely only on reliable things. Don't depend on assumptions. If you can't tell if something is reliable, assume the worst
	- Document your assumptions
	- Don't just test your code, but test your assumptions as well. Don't guess; actually try it. Write an assertion in the code
	- Prioritize your effort. Spend time on the important aspects; more than likely, these are the hard parts
	- Don't be a slave to history. Don't let existing code dictate future code.
### Topic 39 - Algorithm Speed
- If it's tricky getting accurate timings, use *code profilers* to count the number of times the different steps in your algorithm get executed, and plot these figures against the size of the input
- Also be wary of *premature optimization*. It's always a good idea to make sure an algorithm really is a bottleneck before investing your precious time trying to improve it.
### Topic 40 - Refactoring
- Defined by Martin Fowler: 
		A disciplined technique for restructuring an existing body of code, altering its internal structure without changing its external behavior
- Any number of things may cause code to qualify for refactoring
	- Duplication
	- Nonorthogonal design
	- Outdated knowledge
	- Usage
	- Performance
	- The test pass
- #book Refactoring: Improving the Design of Existing Code
	- Don't try to refactor and add functionality at the same time
	- Make sure you have good tests before you begin refactoring. Run the tests as often as possible. That way you will know quickly if your changes have broken anything.
	- Take short deliberate steps: move a field from one class to another, split a method, rename a variable. Refactoring often involves making many localized changes that result in a larger-scale change. If you keep your steps small, and test after each step, you will avoid prolonged debugging
### Topic 41 - Test to Code
- We believe that the major benefits of testing happen when you think about and write the tests, not when you run them
- The basic cycle of Test-Driven Development
	1. Decide on a small piece of functionality you want to add
	2. Write a test that will pass once that functionality is implemented
	3. Run all tests. Verify the only failing one is the one you just wrote
	4. Write the smallest amount of code needed to get the test to pass, and verify that the tests now run cleanly
	5. Refactor your code: see if there is a way to improve what you just wrote (the test or the function). Make sure the tests still pass when you're done.
- The idea is that this cycle should be very short: a matter of minutes, so that you're constantly writing tests and then getting them to work.
- We strongly believe that the only way to build software is incrementally. Build small pieces of end-to-end functionality, learning about the problem as you go. Apply this learning as you continue to flesh out the code, involve the customer at each step, and have them guide the process.
- Tests can definitely help drive development. But, as with every drive, unless you have a destination in mind, you can end up going in circles
- We like to think of unit testing as *test again contract*. We want to write test cases that ensure that a given unit honors its contract
- (in reference to ad hoc testing) At the end of the debugging session, you need to formalize this ad hoc test. If the code broke once, it is likely to break again. Don't just throw away the test you created; add it to the existing unit test arsenal
- Test Window - Log files containing trace messages are one such mechanism. Log messages should be in a regular, consistent format; you may want to parse them automatically to deduce processing time or logic paths that the program took. Poorly or inconsistently formatted diagnostics are just so much "spew" - they are difficult to read and impractical to parse
### Topic 42 - Property-Based Testing
- There are also code *invariants*, things that remain true about some piece of state when it's passed through a function. For example, if you sort a list, the result will have the same number of elements as the original - the length is invariant.
- Once we work out our contracts and invariants we can use them to automate our testing. What we end up doing is called *property-based testing*
- Python - Hypothesis tool with Pytest can run these tests
- Hypothesis will run the test multiple times using in different inputs from the expected list. 
### Topic 43 - Stay Safe Out There
- Analyze the code for ways it can go wrong and add those to your test suite. You'll consider things such as passing in bad parameters, leaking or unavailable resources that sort of thing
- In the good old days, this evaluation of internal errors may have been sufficient. But today that's only the beginning, because in addition to errors from internal causes, you need to consider how an external actor could deliberately screw up the system. But perhaps you protest, "Oh, no one will care about this code, it's not important, no one even knows about this server..." It's a big world out there, and most of it is connected. Whether it's a bored kid on the other side of the planted, state-sponsored terrorism, criminal gangs, corporate espionage, or even a vengeful ex, they are out there aiming for you. The survival time of an unpatched, outdated system on the open net is measure in minutes - or even less.
- Security Basic Principles
	1. Minimize attach surface area
	2. Principle of least privilege
	3. Secure defaults
	4. Encrypt sensitive data
	5. Maintain security updates
- Code complexity makes the attack surface larger, with more opportunities for unanticipated side effects
- The default settings on your app, or for your users on your site, should be the *most* secure values
### Topic 44 - Naming Things
- We believe that things should be named according to the role they play in your code
- It's important that everyone on the team knows what these words mean, and that they use them consistently
	- One way is to have a project glossary, listing the terms that have special meaning to the team. This is an informal document, possibly maintained on a wiki, possibly just index cards on a wall somewhere
## Chapter 8 - Before the Project
- No matter how well thought a project is, and regardless of which "best practices" it includes, no method can replace *thinking*.
### Topic 45 - The Requirements Pit
- Customers don't know what they want. That's where programmers come in. Our job is to help people understand what they want. In fact, that's probably our most valuable attribute
- Sometimes you honestly won't know enough about the domain to know what requirements are missing from a customer request. In those cases, Pragmatic Programmers rely on the "is this what you meant?" school of feedback (during development)
- The Pragmatic Programmer looks at *all* of the project as a requirements gathering exercise. That's why we prefer short iterations; ones that end with direct client feedback. This keeps us on track, and makes sure that if we *do* go in the wrong direction, the amount of time lost is minimized
- We believe that the best requirements documentation, perhaps the *only* requirements documentation, is working code. But, that doesn't mean that you can get away without documenting your understanding of what the client wants. It just means that those documents are not a deliverable: they are not something that you give to a client to sign off on. Instead, they are simply mileposts to help guide the implementation process
- Requirements have to be written down, simply because developers on a team need to know what they'll be doing
- Good requirements are abstract. Where requirements are concerned, the simplest statement that accurately reflects the business need is best. This doesn't mean you can be vague - you must capture the underlying semantic invariants as requirements, and document the specific or current work practices as policy
- Requirements are not architecture. Requirements are not design, nor are they user interface. Requirements are *need*
### Topic 46 - Solving Impossible Puzzles
- Some constraints are *absolute*; others are merely *preconceived notions*
- When faced with an intractable problem, enumerate *all* the possible avenues you have before you. Don't dismiss anything, no matter how unusable or stupid it sounds. Now go through the list and explain why a certain path cannot be taken. Are you sure? Can you *prove* it?
- Perhaps you are running late on the schedule now, or even despair of ever getting the system to work because this particular problem is "impossible." This is an ideal time to do something else for a while. Work on something different. Go walk the dog. Sleep on it.
- Study... - people who were distracted did better on a complex problem-solving task than people who put in conscious effort. If you're still not will to drop the problem for a while, the next best thing is probably finding somebody to explain it to (or simply rubber ducking). Often, the distraction of simply talking about it will lead you to enlightenment. Have them ask you questions such as:
	- Why are you solving this problem?
	- What's the benefit of solving it?
	- Are the problems you're having related to edge cases? Can you eliminate them?
	- Is there a simpler, related problem you can solve? 
### Topic 47 - Working Together
### Topic 48 - The essence of Agility
- Agile values - We are uncovering better ways of developing software by doing it and helping others do it. Through this work we have come to value:
	- **Individuals and interactions** over processes and tools
	- **Working software** over comprehensive documentation
	- **Customer collaboration** over contract negotiation
	- **Responding to change** over following a plan
- What do we do?
	1. Work out where you are
	2. Make the smallest meaningful step towards where you want to be
	3. Evaluate where you end up, and fix anything you broke
## Chapter 9 - Pragmatic Projects
### Topic 49 - Pragmatic Teams
- *Old Systems Maintenance*
	- While we love working on the shiny new system, there's likely maintenance work that needs to be done on the old system. We've met teams who try to shove this work in the corner. If the team is charged with doing these tasks, then do them - for real
- *Process Reflection and Refinement*
	- Continuous improvement can only happen when you take the time to look around, figure out what's working and not, and then make changes. Too many teams are so busy bailing out water that they don't have time to fix the leak. Schedule it. Fix it
- *New tech experiments*
	- Don't adopt new tech, frameworks, or libraries just because "everyone is doing it," or based on something you saw at a conference or read online. Deliberately vet candidate technologies with prototypes. Put tasks on the schedule to try the new things and analyze results.
- *Learning and skill improvements*
	- Personal learning and improvements are a great start, but many skills are more effective when spread team-wide. Plan to do it, whether it's the informal brown-bag lunch or more formal training sessions
### Topic 50 - Coconuts don't cut it
### Topic 51 - Pragmatic Starter Kit
- These are the three legs that support every project
	- Version control
	- Regression testing
	- Full automation
- After you have written a test to detect a particular bug, *cause* the bug deliberately and make sure the test complains. This ensures that the test will catch the bug if it happens for real
- If you are *really* serious about testing, take a separate branch of the source tree, introduce bugs on purpose, and verify that the tests will catch them. At a higher level, you can use something like Netflix's *Chaos Monkey* to disrupt services and test your application's resilience
- Test Coverage - What *is* important is the number of states that your program may have. States are not equivalent to lines of code
- If a bug slips through the net of existing tests, you need to add a new test to trap it next time
### Topic 52 - Delight Your Users
- Our goal as developers is to *delight users*
- Ask customers - How will you know that we've all been successful a month (or a year) after this project is done? 
### Topic 53 - Pride and Prejudice
- Pragmatic Programmers don't shirk from responsibility. Instead, we rejoice in accepting challenges and in making our expertise well known. If we are responsible for a design, or a piece of code, we do a job we can be proud of