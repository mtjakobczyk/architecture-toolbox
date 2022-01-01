## 97 Things Every Software Architect Should Know
<img src="https://learning.oreilly.com/covers/urn:orm:book:9780596800611/400w/" alt="drawing" width="150"/>

Source for all quotes: https://learning.oreilly.com/library/view/97-things-every/9780596800611/

### My notes and my favourite quotes from the book

#### 1. Don’t Put Your Resume Ahead of the Requirements (Nitin Borwankar)
> It’s often difficult to resist utilizing a solution that is new and cool, even when it’s inappropriate for the current situation.
 
> The best thing for your career is a long string of happy customers eager to recommend you because you did the right thing by them and for the project.

> Always put the customer’s long-term needs ahead of your own short-term needs and you won’t go wrong.

#### 2. Simplify Essential Complexity; Diminish Accidental Complexity (Neal Ford)

> Essential Complexity represents the difficulty inherent in any problem. 

**Essential Complexity** is the nature or a property of a problem. To solve the problem, you need to approach and handle all the essential complexity. There is no way to avoid it.
Example: *To build a financial reporting system, you have to understand the domain, all related constraints and the options you have.*

> accidental complexity grows from the things we feel we must build to mitigate essential complexity

While solving a problem, you choose tools, techniques and patterns which may introduce additional complexity called **accidental complexity**. Example: *If you decide to build a financial reporting system using microservices, you need to put additional effort in enforcing saga-based transactionality across these loosely couples components.* 

> Many frameworks and vendor “solutions” are the symptoms of the accidental complexity disease. Frameworks that solve specific problems are useful. Over-engineered frameworks add more complexity than they relieve.

> It’s the duty of the architect to solve the problems inherent in essential complexity without introducing accidental complexity.

> Prefer frameworks derived from working code rather than ones cast down from ivory towers

#### 3. Chances Are, Your Biggest Problem Isn’t Technical (Mark Ramm)
> There’s a good chance that there’s someone who you think is “just not doing it right” and is undermining the project

> What you need is a conversation.
> 1. Approach these events as conversations—not as confrontations.
> 2. Approach these conversations only after you’ve got your attitude right.
> 3. Use these as opportunities to set mutually agreed-upon goals.

> If you start with a shared purpose, treat people “problems” as an opportunity to learn, and manage your own emotions, you’ll not only become more effective, you’ll also discover that you learn something every time.

#### 4. Communication Is King; Clarity and Leadership, Its Humble Servants (Mark Richards)
> Every software architect should know how to communicate the goals and objectives of a software project.

> All too often, software architects sit in their ivory towers, dictating specifications, technology decisions, and technology direction to the developers below

> Clarity describes how you communicate. No one on your team is going to read a 100-page architecture decisions document.  
> Create simple diagrams to convey your thoughts. Keep them simple, for they will almost certainly be changing frequently.

> Keeping developers in the dark about the big picture or why decisions were made is a clear recipe for disaster.  
> Having the developer on your side creates a collaborative environment whereby decisions you make as an architect are validated.

#### 6. Seek the Value in Requested Capabilities (Einar Landre)

> Often customers and end users state **what they think** is a viable solution to a problem as a requirement.

> By asking for **the intended value** of a requested feature or requirement, architects are able to **address the real problem**, and hopefully provide a better and cheaper solution than that suggested by the client.

> In many ways the required approach is found in the agile manifesto: “Collaboration over contract.” Practically speaking, this implies arranging workshops and meetings where the architects’ focus is on customer needs—helping the customers to answer the “why” question

#### 10. Quantify (Keith Braithwaite)

> “Fast” is not a requirement. Neither is “responsive.” Nor “extensible.”  
> You have no objective way to tell if they’re met.

> Without objective criteria, architects are at the mercy of capricious users and of obsessive programmers 

> Uncertain quantitative criteria must be given as a range: the least, the nominal, and the most.

#### 11. One Line of Working Code Is Worth 500 of Specification (Allison Randal)

> it’s far too easy to get wrapped up in the process of design, enthralled by architecture in abstract.  
> The fact is that **specifications alone have no value**. The ultimate goal of a software project is a production system.

> Value the team members who work on implementing your vision. Listen to them. When they have problems with the design, there’s a good chance they’re right and the design is wrong, or at least unclear.

> No design is perfect from the start; all designs need to be modified as they are implemented.

#### 12. There Is No One-Size-Fits-All Solution (Randy Stafford)

> People are often responsible for solving problems requiring more contextual sense than they’ve accumulated.

> Architects must develop and exercise contextual sense in formulating and troubleshooting their architectures

#### 17. Business Drives (Dave Muirhead)

> An architect must act as **a bridge between the business and technology communities** of an organization: 
> - representing and protecting the interests of each party to the other, 
> - often mediating between the two, 
> - but **allowing the business to drive**

> Part of the challenge of letting the business “drive” is providing enough quality information about the ongoing software development effort back into the business. Transparency becomes crucial. The architect, in conjunction with development management, must create and nurture the means for regular, ongoing information feedback loops. 

#### 18. Simplicity Before Generality, Use Before Reuse (Kevlin Henney)

> Favoring simplicity before generality acts as a tiebreaker between otherwise equally viable design alternatives.  
> When there are two possible solutions, favor the one that is **simpler and based on concrete need** rather than the more intricate one that boasts of generality

> Too often **generalization becomes a work item in itself**, pulling in the opposite direction, adding to the complexity rather than reducing it.

Generalization is often introducing considerable degree of accidental complexity.

#### 19. Architects Must Be Hands On (John Davies)

> A good architect should lead by example. He (or she) should be able to fulfill any of the positions within his team.

> Without a good understanding of the full range of technology, an architect is little more than a project manager.  

> It is perfectly acceptable for team members to have more in-depth knowledge in their specific areas but it’s difficult to imagine how team members can have confidence in their architect if the architect doesn’t understand the technology.

#### 27. There Is No ‘I’ in Architecture (Dave Quick)

> Our egos can be our own worst enemy.

> I suspect any experienced architect has fallen into at least one of these traps at some point:
> 1. think they understand the requirements better than the customers
> 2. view developers as resources hired to implement their ideas
> 3. get defensive when their ideas are challenged
> 4. ignore the ideas of others

> Removing the ‘I’ from architecture removes a common source of failure that’s entirely your fault.

#### 28. Get the 1,000-Foot View (Erik Doernenburg)

> In an architecture diagram, little boxes represent entire systems and lines between them can mean anything: a dependency, the flow of data, or a shared resource such as a bus. These diagrams are a **30,000-foot view**, like a landscape seen from a plane.

> Typically the only other view available is the source code, which is comparable to a **ground-level view**.

> Both views fail to convey much information about the quality of the software: 
> - one is too high level and 
> - the other provides so much information that we cannot see structure.

> Clearly, what is missing is a view in between—a **1,000-foot view**. This 1,000-foot view would provide information at the right level.

#### 29. Try Before Choosing (Erik Doernenburg)

> A stereotypical architect might gather all the information that can be gathered, then mull over it for a while, and finally decree the solution from the ivory tower for it to be implemented by the developers.

> The architect should constantly be on the lookout for decisions that will have to be made soon

> Trying two or even more approaches to the same problem requires more effort than making a decision upfront and then just implementing one. However, chances are that an upfront decision leads to a solution that is later recognized to be suboptimal.

Prototype to make a decision!

#### 30. Understand the Business Domain (Mark Richards)

> Effective software architects understand not only technology but also the business domain of a problem space. 
> 
> Without business domain knowledge, it is difficult to understand the business problem, goals, and requirements, and therefore difficult to design an effective architecture to meet the requirements of the business.

> As a software architect, always understand the goals of the company you are working with, and validate that the architecture can support these goals.

> The most successful architects I know are those who have broad hands-on technical knowledge coupled with a strong knowledge of a particular domain

#### 32. Give Developers Autonomy (Philip Nelson)

> Most architects begin their careers as developers. An architect has new responsibilities and greater authority in determining how a system is built. 
> 
> As a developer you rarely get the time to sit back and really look at how the whole system fits together. As an architect, this is your main focus.

> If you’re doing a great job of being an architect, you: 
> - do need to watch closely enough to see that the design is being implemented as intended. 
> - do not need to be standing over people’s shoulders to accomplish that goal. 
> It’s reasonable to make suggestions when you see people struggling, but it’s even better if you create the environment where they come and ask you for suggestions.

#### 35. Scope Is the Enemy of Success (Dave Quick)

> Scope refers to a project’s size. How much time, effort, and resources? What functionality at what level of quality? How difficult to deliver? How much risk? What constraints exist? The answers define a project’s scope.

> Expanding scope is the enemy of success because the probability of failure grows faster than expected

> Strategies that can help to reduce or manage scope in real-world projects:
> - Understand the real needs
> - Divide and conquer - *Look for opportunities to divide up the work into smaller independent chunks*
> - Prioritize - *Prioritization lets you deliver the most important requirements first*
> - Deliver results as soon as possible

> Complex architectures fail far more often than simpler architectures. Reducing project scope often results in a simpler architecture

#### 36. Value Stewardship Over Showmanship (Barry Hawkins)

> When an architect enters a project, there is an understandable desire to prove his or her worth.
>
> **Showmanship**, the act of appealing to your audience, is important in marketing, but it’s counterproductive to leading a software development project

> Architects must win the respect of their team by providing solid leadership and by truly understanding the technical and business domain in which they are expected to operate.
>
> **Stewardship**, taking responsibility and care of another’s property, is the appropriate role of an architect

> Value stewardship over showmanship; never forget that you are playing with other people’s money.

#### 43. Context Is King (Edward Garson)

> Context is king, and simplicity its humble servant. 
> 
> What this means in practical terms is that context is the only force that trumps simplicity when you’re making architectural decisions.

> Good architecture is the product of decisions made within a context usually tainted with multiple **competing priorities**. 
> Those competing priorities mean that sometimes **the most important decisions are not about what you put in, but rather what you omit**.

#### 47. Welcome to the Real World (Gregor Hohpe)

> Engineers like **precision**, especially software engineers who live in the realm of ones and zeros. They are used to working with binary decisions, one or zero, true or false, yes or no. Everything is clear and consistent, guaranteed by foreign key constraints, atomic transactions, and checksums.

> The real world is not quite that binary. Widely distributed systems introduce a whole new set of inconsistencies into the game

> Say goodbye to the good old predictive call-stack architecture, where you get to define what happens when and in what order. 
> 
> Instead, be ready to **respond to events at any time in any order**, regaining your context as needed. 
> 
> Avoid complete chaos by modeling your application using **event-driven process chains** or **state models**. Reconcile errors through compensation, retry, or tentative operations.

#### 50. Architects’ Focus Is on the Boundaries and Interfaces (Einar Landre)

> From separation of concern we get encapsulation, and from encapsulation we get boundaries and interfaces.
> 
> Here the concept of **bounded contexts** and **context mapping**, as described by Eric Evans in his book Domain-Driven Design (Addison-Wesley Professional), comes to the rescue.
> 
> A **bounded context** is an area where a model or concept is uniquely defined. With the bounded contexts identified and drawn up on the whiteboard, it’s time to start to draw the relationships between the contexts. The result from this exercise is a **context map**, a collection of bounded contexts and the interfaces between them.

#### 51. Empower Developers (Timothy High)

> The role of an architect is usually to impose constraints, but you also have the opportunity to **be an enabler**.
> 
> You should do everything possible to empower your developers. Make sure developers have the **tools** they need. Make sure they have the **skills** they need. Let developers make **their own decisions** wherever it won’t contradict the overall goal of the software design. Protect developers from **nonessential parts** of their job

#### 52. Record Your Rationale (Timothy High)

> Software architecture is all about choosing the right tradeoffs between various quality attributes, cost, time, and other factors. 
> 
> It should be made clear to you, your managers, developers, and other software stakeholders why one solution was chosen over another and what tradeoffs this entailed.

> The documentation should answer the basic questions “What was that decision we made?”, and “Why did we make that decision?”. A secondary question that is often asked and should be documented is “What other solutions were considered, and why were they rejected?”


#### 53. Challenge Assumptions—Especially Your Own (Timothy High)

> Best practices in software architecture state that you should document the rationale behind each decision that is made, especially when that decision involves a tradeoff. This practice is valuable because listing these factors helps highlight assumptions.
>
> It is important to make these assumptions visible and explicit for the sake of posterity and for future re-evaluation
> 
> Very often assumptions are based on “historical reasons,” opinion, developer lore, FUDs, or even “something I heard in the hallway”

#### 55. Pattern Pathology (Chad LaVigne)

> Design patterns are excellent tools for mitigating necessary complexity, but like all tools, they can be misused. 
> 
> Design patterns become a problem when we make them the proverbial hammer with which we must strike every nail. Be careful that your appreciation for patterns doesn’t become an infatuation that has you introducing solutions that are more complicated than they need to be.
> 
> Stamping patterns all over a project unnecessarily is over-engineering.

#### 57. Focus on Application Support and Maintenance (Mncedisi Kasper)

> The support and maintenance of an application should never, ever be an afterthought.
> 
> You should pay a lot of attention to the problems of support and maintenance when you’re designing

#### 60. Start with a Walking Skeleton (Clint Shank)

> One very useful strategy for implementinh, verifying, and evolving an application architecture is to start with what Alistair Cockburn calls a **walking skeleton** - a minimal, end-to-end implementation of the system that links together all the main architectural components. 

> Start with a walking skeleton, keep it running, and grow it incrementally. The bigger the system, the more important it is to use this strategy.

#### 61. It Is All About The Data (Paul W. Homer)
> Data sits at the core of most problems. Business domain problems creep into the code via the data.
> 
> From a design perspective, the critical issue for most systems is to **get the right data into the system at the right time**.
>
> This data-oriented perspective—seeing the system entirely by the structure of its underlying information—can reduce even the most complicated system down to a tangible collection of details.

#### 65. Your System Is Legacy; Design for It (Dave Anderson)

> Even if your system is bleeding edge and developed in the latest technology, it will be legacy to the next guy. Deal with it!
>
> Legacy tends to be a bad word in software circles, but in reality, all software systems should endure the tag. It is not a bad thing, as it may indicate that your system is durable, meets expectations, and has business value.
>
> If you expect your system to go into production and survive, even for a few months, then you need to accept that maintenance developers will need to fix things up.

#### 69. Shortcuts Now Are Paid Back with Interest Later (Scot Mcphee)

> Shortcuts taken during the initial development phase of a project can result in significant maintenance costs later.
>
> A serious architectural mistake is to adapt an existing system for a purpose that it is not fit for, on the basis that using an existing system somehow reduces costs.
> 
> Poorly designed features can become the foundation for future features, making corrective action later even more costly.

#### 70. “Perfect” Is the Enemy of “Good Enough” (Greg Nyberg)

> Don’t give in to the temptation to make your design, or your implementation, perfect! The search for perfection in design and implementation leads, in my opinion, to overdesigned and obfuscated solutions that are, in the end, harder to maintain.
>
> Aim for “good enough” and stop when you’ve achieved it. Good enough means that the remaining imperfections do not impact system functionality, maintainability, or performance in any meaningful way.

#### 87. Pay Down Your Technical Debt (Burkhardt Hufnagel)

> Generally, the business people will want the change made as quickly as possible, while the developers and testers will be more interested in taking the time to properly design, implement, and test the change before delivering it to the customers.
>
> As the project’s architect, you’ll have to decide which makes more sense and then convince the decision makers to take your advice; and, as with most architectural issues, there is a tradeoff involved

> If you believe the system is reasonably stable, then it may make sense to go the “quick and dirty” route and get the change into production quickly. That’s fine, but you need to know that in doing so your project is incurring some “technical debt” that must be repaid later.
> 
> For technical debt, interest takes the form of instability in the system, and increased maintenance costs due to the hacked-in changes and lack of proper design, documentation, and/or tests. 

#### 88. Don’t Be a Problem Solver (Eben Hewitt)

> With some exceptions, architects used to be developers. Developers get rewarded for solving programming problems, which are more local in scope than architectural problems.
> 
> Architects and developers learn to enter problem-solving mode immediately. But sometimes the best solution is no solution.
> 
> Because architects tend to immediately enter problem-solving mode, we forget, or rather have never learned how, to **interrogate the problem itself**
>
> We must learn, like a telephoto lens, to **zoom in** and **zoom out**, in order to **ensure that the question is really framed properly**, and that we’re not merely accepting what we’re given.

#### 96. For the End User, the Interface Is the System (Vinayak Hegde)

> There are too many good products hidden behind bad user-interfaces.
>
> If the quality of the user’s experience while interacting with your product suffers, then his impression of your product will suffer, no matter how technologically advanced and path-breaking your product might be.

> **User interaction** should be an integral part of the decision-making process for architecture tradeoffs and internal product documentation as much as robustness and performance.

#### 97. Great Software Is Not Built, It Is Grown (Bill de hÓra)

> Have a grand vision, but not a grand design.
> 
> Resist trying to design a large complete system to “meet or exceed” the known requirements and desired properties, no matter how tempting that might be.

> Design the smallest system you can, help deliver it, and let it evolve toward the grand vision. 
> 
> Inducing a system to evolve means starting with a small running system, a working subset of the intended architecture—the simplest thing that could possibly work.
