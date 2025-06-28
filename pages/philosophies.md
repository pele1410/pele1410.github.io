# What I Believe

## General Philosophies

> It is on men that safety at sea depends and they cannot make a greater mistake than to suppose that machines can do all their work for them
>
> ~Mr. Justice Cairns, 1967

It is my job to prove this man wrong.

### Asking Questions

Many people, especially junior developers, fear that they'll look stupid if they ask questions. My general response to that is... <i>Get over it</i> . If you don't ask questions, you won't get answers and that will be worse in the long run.

> It's better to ask questions and look stupid now than not ask questions and remain ignorant forever"
>
> ~somebody on the internet.

### Doing something bad is usually better than doing nothing at all
Seems counterintuitive, but atleast trying something and failing will be better in the long run than never trying. You can learn from mistakes, you can't learn from doing nothing.

### Make it work, then make it pretty

When developing something new there is a lot to gain by rapidly getting something working and then focusing on making it pretty and supportable long-term.  We should strive for getting a working POC in the field within a few sprints so we can have something landable that can be reviewed. Then we can iterate rapidly on changes or improvements as necessary while having trust that the core is correct. This is not to say you should hack something together and call that a POC; it should be designed properly still. The intent is to get the core skeleton in place and approved/tested without waiting until 90% of the work is completed.

## Testing

### Test Early, Test Often

While not explicitly advocating for Test Driven Development (TDD), I’m a big fan of it.

Crafting tests can help drive error handling and verification

Knowing how you will test before starting implementation provides insight into what the code should be accomplishing

Maintaining passing tests ensures code doesn’t break

Maintaining passing tests allows for incremental changes to be tested easily during development

Maintaining a system that is functional enough to be tested ensures we can always test

### Test Happy Paths AND Unhappy Paths

Anyone can write a function that does what it’s supposed to with expected sane input. But good functions manage garbage gracefully and good tests ensure that

### Fail Fast, Fail Hard

Failures should happen as soon as they are identified.  This makes it easier to see where the root case occurred instead of 5 layers above.

Failures should be loud; obvious to everyone.  This ensures that failures do not go unnoticed and lead to undefined behavior in the software.  Failing loudly also means that failures will be more likely to be found during testing phase and not in production.

### Missing Something?

Don’t have an engine service to use? Make one.

Need a fake service to stub out functionality? Make one

Stubs help everyone, not just you. And they help in all types of testing

### Repeatability

Tests should be easily repeatable, by anyone, at any time

### If It's Not Broken, It's Not Tested Enough

Software will be broken somehow. The job of a tester is to be able to find exactly where and how the software is broken. It may not always be a major breakage, but something somewhere will not function perfectly correct. If you haven't found that yet, then you haven't tested enough.
