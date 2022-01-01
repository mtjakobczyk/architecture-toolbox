## 97 Things Every Software Architect Should Know
<img src="https://learning.oreilly.com/covers/urn:orm:book:9780596800611/400w/" alt="drawing" width="150"/>

Source for all quotes: https://learning.oreilly.com/library/view/97-things-every/9780596800611/

### My notes and favourite quotes

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

