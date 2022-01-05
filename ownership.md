## Definition

**Ownership over a decision means that you can make or change the decision unilaterally, without consensus, but others will expect you to understand and explain it**

## Code Ownership

The form of ownership with which you're most familiar may be code ownership. When you "own" a piece of the codebase, then others expect you to know how it works and why it works that way[^1]. You implement its feature requests, review its PRs, and answer questions about how it works. Ideally, two or more people own every part of the codebase; they trust each other—or at least negotiate with each other—to make decisions, and they communicate regularly about decisions made. They can review each others' code and cover for each other during vacations or other absences.

Code ownership is a special case of decision ownership. The need to make lots of open-ended decisions fundamentally defines creative work in general; in software specifically, the open-ended decisions look like: what are the variables called? How is the code laid out? What's the API? Etc. When you own a piece of the codebase, you own those decisions. By extension, if you need to make changes to another part of the codebase, one of the owners of that code needs to review it. They're responsible for the decisions in your PR, so try to accommodate their requests.

Engineers looking for more autonomy or to grow their career should look for parts of the codebase they can own. Many sections of most codebases eventually get neglected by owners too busy to pay them much attention. Those sections of code often use old libraries or contain redundant implementations. If you use the autonomy of ownership to rewrite such code (typically alongside or with guidance from the prior owner), then you'll know how it works, making you a good owner.

If you've been at Pachyderm for a while and want to lighten your load, don't be afraid to hand off code ownership to new engineers or to other teams more invested in that code. They might rewrite it and you might lose your understanding of how it works, but if you're not the owner, you're not responsible for those changes. Focusing more energy on fewer projects is a great way to increase your productivity, and productively developing high-impact projects is a great way to grow your career. Meanwhile, the old library you grudgingly maintain, which distracts you from your more ambitious projects, may be critical to someone else's grand vision. Be nice to the new owners though; they're inheriting the code's existing decisions, which you'll still understand best for a while.

## Non-Code Ownership

There are many decisions made at Pachyderm about things other than code: What do we put on the product's roadmap? How will we market it? What's our release process? What do we prioritize? Who do we hire? These, in a sense, constitute the broader creative project that is a software product, or even the creative project that is Pachyderm the company. Those decisions should have owners too. If you'd like to change one of them, find out who the owners are and work with them, as you would when sending a PR. Or, if you are the owner, change it!

## Ownership Ownership

Finding owners is one of the main decisions that managers make. Managers normally shouldn't make decisions over which they have delegated ownership, but it's reasonable for them to ask how a decision serves the company's goals, and if the company's goals aren't getting accomplished, it's reasonable to change the owner of those decisions in order to try a new approach.

[^1]: If you're new to code ownership: it's okay if your code is bad for a bad reason, e.g. "we were in a hurry so we copied a bunch of code from another part of the codebase." Obviously that situation isn't ideal, but your job is just to know that fact! Realistically, we will write bad code sometimes for a variety of reasons, and because you know the reason, others won't be afraid to rewrite it when they have more time, knowledge, or motivation.
