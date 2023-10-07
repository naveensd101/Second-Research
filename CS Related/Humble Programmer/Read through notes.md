# Humble Programmer

## Page 1

- Year in context is 1960s.
- Talks about how programmers have nothing sexy like the electronics people that we can show about our work.
- Our work is mere strings of words (something like a movie script I would say).
  - We have our syntax and semantics (like English language)
  - We play with it
- In old days more emphasis was given to computers and not to the programmer
- Machines were very limited by memory, compute power etc.
- This made programmers to invent clerver tricks to do problems
- Naive us thought that programming as such will dissapear when compute power increases
- But fast forward 10yrs (this should be the year 1970s). We are in the middle of a software crisis

## Page 2

- Starts to talk about why in 1970s we had a software crisis.
- This page takes a huge jump in a knowledge standpoint
- To understand what he EWD is talking about we should know how an Operating System works.
- Talks about **Minor Cause**.
  - Computers became more complicated
  - *I/O interupts* happening at random intervals
  - But for a 2020s guy my whole life is this.
  - IDK what the *old sequentail machine* is
  - *Multi Level memory*
  - again thats my whole life for 2020 person
  - He tells that in 1970s multi level caching was a big deal. Even after extensive literatures on the topic. He tells its elusive
  - Jesvin explaned about how *Computer Architecture* coures in NITC just went over his head after a point. There were a lot of caches and cores for him to keep track with
  - *Is 1972 artcicle still valid for us then*
- But this problem was mentioned to be a **Minor** problem by Dijkstra
- Major flaw is the computer getting more powerful.
- Then Dijkstra talks about how hardware are consentrating on price to performance ration.
- And they can use a crappy instruction set architecture and bring the price to performance value up.
- But it will be a pain in the ass to programe in
- He also mentions that how we review papers in CS theory. We should also review computer hardware that come new.
- 3rd generation computers
  - Dijkstar mentions it >1 times now itself.
  - We are currently in 5th geneartion
  - dem i think i remember reading a bit about it in my school 11th textbook first chapter
  - I went to my old textbook pile and got it.
![school textbook cover](sumita.jpeg)
![chapter on computer generations](sumita-computer-geneartion.jpeg)
  - It didn't give much help.
  - First generations used Vacume tubes
  - Second generations used Transistors
  - 3rd Generation used ICs - At this point we started using C language.
  - 4th Generation
  - 5th Generation
- Dijkstra tells that 3rd generation computers were flawed.
  - Can you give me why it was so? Are the flawes still prevelent in todays computers?
  - Dijkstra mentions that the instruction set of the 3rd generation PCs were bad.
  - By 3rd generation i believe that the assembly language was standardised.

## Page 3

- Starts off talking about software problems.

### EDSAC

- Used subroutines (functions). which is good design
- **Functions** are one of the *greatest software inventions*

> Regrettably enough, its importance has been underestimated in the design of the third generation computers, in which the greate number of explicitly named registers of the arithmetic unit implies a large overhead on the subroutine mechanism.

- I dont understand what dijkstra is tyring to point out.

### FORTRAN

> The sooner we can forget that FORTRAN ever existed, the better, for as a vehicle of thought it is no longer adequate: it wastes our brainpower, and it is too risky and therefore too expensive to use.

- Why so much hate for FORTRAN?
- I read somewhere that this hate is because FORTRAN disallowed functions.
- I couldn't find a source to validate my claim.

### LISP

- So much love here.

### ALGOL 60

- My understanding: Fortran's differes according to its implementation in different architecture. But Algol 60 was defined as a language independed of implementation. Hmm thats interesting.

### PL/1

- Has way many features to keep track of.

## Page 4

- Decides to stop rant about old stuff.
- Dijkstra's vision for 1970 - 79

> well before the seventies have run to completion, we shall be able to design and implement the kind of systems that are now straining our programming ability at the expense of only a few percent in man-years of what they cost us now, and that besides that, these systems will be virtually free of bugs.
> If you want more effective programmers, you will discover that they should not waste their time debugging = they should not introduce the bug to start with.

- Three major conditions for this revolution to be successful.

1. The world at large must recognize the need for the change.
2. The *economic* need for it must be sufficiently strong.
3. The change must be *technically feasible*.

### World's acceptance of the issue

- Read more about software crisis [here](https://en.wikipedia.org/wiki/Software_crisis).
- In late 1960s there were a lot of talks about **Software crisis**
- I am not sure about the current state. A few years of industry experience might help me give an answer to this question.
- Dijkstra takes 1st condition to be satsified just as it is because of all the Software crisis talks going on.

### Economic need

> as long as machines were the largest item on the budge, the programming profession could get away with its clumsy techniques; but that umbrella will fold very rapidly.

- We should find a way to make software more cheeply. That is the Economic need.

### Technical Feasibility

- Dijkstra will give six arguments in support that its technically feasible.
- Intelectuall managablility of program
- Mathematical rules and non mathematical rules.

#### Exclusion of goto-statements

- I know that having goto statements will make it hard to make functions with single entry and single exit doors.
- I am not super into the idea of completely avoiding goto statements.

#### Procesduers with >1 output parameters

- I have zero evidence on why this should be true.
- I am gonna have to take this as dijkstra's words. *Hope* that he is correct. He is huge in cs. And i am just starting to know what OS is.

#### Loops should always have a invariant. (non mathemaical rule)

- I have attended a lecture on this topic. I will try to post about it sometime. It talks about how we can formally prove that a loop will terminate when the needed outcome is reached.

- If the above three values are satisfied. The program will be **intellectually manageable**. We should restrict ourseves to *only intellectually manageable problems*.

## 6 Arguments about Technical Feasibility of Software revolution

1. Intellectually manageable problems only
2. By considering intellectually manageable problems, we have drastica reduction of the solution space to be considered. (This argument is different from the first one, but I dont get it)
3. Correctness proof of a program should come before we actually code it. (The only tricky part would be thinking of correctness when fork comes in and data sharing comes. The easiest to learn will be loop invariance)
4. Absolutely precisely defined abstractions.
5. The competent programmer is fully aware of the strictly limited size of his own skull; therefore he approaches the programming task in full humility. As Very Humble Programmers. (This section was really good. Even in 2023 i can say that we do all the bad thinks that Dijkstra points out. Is all of them bad? I am not the best person to answer that yet. But I have learned enought to question it, than blindly following the advice.)

> The tools we are trying to use and the language or notation we are using to express or record our thoughts are the major factors determining what we can think or express at all!

- Avoid one line clever tricks that dont give computational advantage.
- Even using foor loops can affect our thinking. We might not identify a easy elegant and more efficient solution. Since we are so used to using for loops. Where we associate looping with a counter variable.

6. Any big software projects can be factored into smaller manageable independent problems.
