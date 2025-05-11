## Chapter 1 - A Pragmatic Philosophy
 - "What distinguishes Pragmatic Programmers? We feel it’s an attitude, a style, a philosophy of approaching problems and their solutions. They think beyond the immediate problem, placing it in its larger context and seeking out the bigger picture."
### Topic 1 - It's Your life
### Topic 2 - The Cat Ate My Source Code
- "Pragmatic Programmers take charge of their own career, and aren't afraid to admit ignorance or error."
- "Above all, your team needs to be able to trust and rely on you-and you need to be comfortable relying on each of them as well. Trust in a team is absolutely essential for creativity and collaboration according to the [research literature](http://dx.doi.org/10.1037/apl0000110)."
- "Before you approach anyone to tell them why something can't be done, is late, or is broken, stop and listen to yourself"
- "When you find yourself saying, 'I don’t know,' be sure to follow it up with '—but I’ll find out.' It’s a great way to admit what you don’t know, but then take responsibility like a pro."
### Topic 3 - Software Entropy
- "Don’t leave 'broken windows' (bad designs, wrong decisions, or poor code) unrepaired. Fix each one as soon as it is discovered. If there is insufficient time to fix it properly, then board it up. Perhaps you can comment out the offending code, or display a 'Not Implemented' message, or substitute dummy data instead. Take some action to prevent further damage and to show that you’re on top of the situation."
- "don’t cause collateral damage just because there’s a crisis of some sort. One broken window is one too many."
### Topic 4 - Stone Soup and Boiled Frogs
- "You may be in a situation where you know exactly what needs doing and how to do it. The entire system just appears before your eyes—you know it’s right. But ask permission to tackle the whole thing and you’ll be met with delays and blank stares. People will form committees, budgets will need approval, and things will get complicated. Everyone will guard their own resources. Sometimes this is called “start-up fatigue.’’ It’s time to bring out the stones. Work out what you can reasonably ask for. Develop it well. Once you’ve got it, show people, and let them marvel. Then say “of course, it would be better if we added…’’ Pretend it’s not important. Sit back and wait for them to start asking you to add the functionality you originally wanted. People find it easier to join an ongoing success. Show them a glimpse of the future and you’ll get them to rally around."
- "Constantly review what's happening around yo, not just what you personally are doing."
### Topic 5 - Good-Enough Software
- "you can discipline yourself to write software that's good enough for your users for future maintainers,  for your own peace of mind. You'll find that you are more productive and your users are happier. And you may well find tha your programs are actually better for their short incubation"
- "many users would rather use software with some rough edges *today* than wait a year for the shiny, bells-and-whistles version."
- "Don't spoil a perfectly good program by over-embellishment and over-refinement"
### Topic 6 - Your Knowledge Portfolio
- "To be successful in your career, you must invest in your knowledge portfolio using the same guidelines [as investors] (1. Invest regularly. 2. Diversify. 3. Balance portfolios. 4. By low and sell high. 5. Reviewed and rebalanced regularly). The good news is that managing this kind of investment is a skill just like any other-it can be learned. The trick is to make yourself do it initially and for a habit. Develop a routine which you follow unit"
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
- "So you’re reading voraciously, you’re on top of all the latest breaking developments in your field (not an easy thing to do), and somebody asks you a question. You don’t have the faintest idea what the answer is, and freely admit as much. Don’t let it stop there. Take it as a personal challenge to find the answer. Ask around. Search the web—the scholarly parts too, not just the consumer parts. If you can’t find the answer yourself, find out who can. Don’t let it rest. Talking to other people will help build your personal network, and you may surprise yourself by finding solutions to other, unrelated problems along the way. And that old portfolio just keeps getting bigger…."
- "Beware of the zealots who insist that their dogma provides the only answer."
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
- Plan what you want to say. Write an outline. Then as yourself, "Does this communicate what I want to express to my audience in a way that works for them?" Refine it until it does.
- Make what you're saying relevant in time, as well as in context.
- Keeping people informed makes them far more forgiving of the occasional slip, and makes them feel that you haven't forgotten them.
- Finally, there’s the matter of communicating via documentation. Typically, developers don’t give much thought to documentation. At best it is an unfortunate necessity; at worst it is treated as a low-priority task in the hope that management will forget about it at the end of the project. Pragmatic Programmers embrace documentation as an integral part of the overall development process. Writing documentation can be made easier by not duplicating effort or wasting time, and by keeping documentation close at hand—in the code itself. In fact, we want to apply all of our pragmatic principles to documentation as well as to code.
- Commenting source code gives you the perfect opportunity to document those elusive bits of a project that can’t be documented anywhere else: engineering trade-offs, why decisions were made, what other alternatives were discarded, and so on.
- Challenges
	- There are several good books that contain sections on communications within teams, including The Mythical Man-Month: Essays on Software Engineering [Bro96] and Peopleware: Productive Projects and Teams [DL13]. Make it a point to try to read these over the next 18 months. In addition, Dinosaur Brains: Dealing with All Those Impossible People at Work [BR89] discusses the emotional baggage we all bring to the work environment.

Thomas, David; Hunt, Andrew. Pragmatic Programmer, The: Your journey to mastery, 20th Anniversary Edition (p. 70). (Function). Kindle Edition. 
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
-