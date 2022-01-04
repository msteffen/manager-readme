## Definition

**Ownership over a decision means that you can make or change the decision unilaterally, without consensus, but others will expect you to understand and explain it**

## Code Ownership

I believe code ownership is the most widely-practiced form of ownership in the tech industry. As an engineer, if you "own" a piece of the codebase, then you know how it works. You implement its feature requests, review its PRs, and answer questions about how it works. Ideally, two or more people own every part of the codebase (they'll need to trust each other, or at least negotiate with each other, to make decisions, and communicate regularly about decisions made. But, they also cover for each other during vacations or other absences).

Code ownership is a special case of decision ownership. The defining characteristic of all creative work is the need to make lots and lots of open-ended decisions; in software, decisions look like: what are the variables called, how is the code laid out, etc. When you own a piece of the codebase, you own those decisions. By extension, if you need to make changes to another part of the Pachyderm codebase, the owner of that code needs to review it. They're responsible for the decisions in your PR, so try to accommodate their requests.

Engineers looking for more autonomy or to grow their career should look for parts of the codebase they can own. There are many sections of code where the owner is too busy to pay them much attention. Those sections of code have often buried bitrotted, using old libraries and redundant implementations. If you use the autonomy of ownership to rewrite one (typically alongside or with guidance from the prior owner), then you'll know how it works, making you a good owner.

If you've been at Pachyderm for a while and want to lighten your load, don't be afraid to hand off code ownership to new engineers or to other teams who have more stake in that code. They might rewrite it and you might lose your understanding of how it works, but if you're not the owner, you're not responsible for those changes. Focusing more energy on fewer projects is also a great way to increase your productivity. Be nice to the new owners though; they're inheriting the code's existing decisions, which you'll still understand best for a while.

## Non-code Ownership

There are many decisions made at Pachyderm about things other than code: what is our product's roadmap? How will it be marketed? What is our release process? What are our team's priorities? Who do we hire? These, in a sense, are part of the broader creative project that is a software product, or even the creative project of Pachyderm the company. Those decisions should have owners too. If you'd like to change one of them, find out who the owner is and work with them. Or, if you are the owner, change it!

## Ownership ownership

Finding owners for decisions is the responsibility of Pachyderm's leadership, and delegating that ownership is one of the main parts of their jobs. Managers shouldn't be making any decisions over which they have delegated ownership, but it's reasonable for them to ask how a decision serves the company's goals, and if the company's goals aren't getting accomplished, it's reasonable to change the owner of decisions that aren't working.
