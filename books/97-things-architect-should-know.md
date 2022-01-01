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
