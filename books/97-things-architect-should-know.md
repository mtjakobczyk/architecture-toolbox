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
