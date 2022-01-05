Sources: [Write More Tests, Part 1](https://writemoretests.com/2012/02/how-to-estimate-like-adult-part-1.html), [Part 2](https://writemoretests.com/2012/02/estimating-like-an-adult-what-to-steal-from-agile.html), [An Epic Treatise on Scheduling, Bug Tracking, and Triage](https://apenwarr.ca/log/20171213)

### Observation

An empirical claim: if Staff Engineer Alice takes a day to implement a feature that would have required a week from Junior Engineer Bob, then that 5x ratio generalizes to other projects. Bob will typically take 5x as long to implement a feature as Alice would.

### Story Points

Given the observation above, it would make sense to estimate project duration by first estimating the project's size in "abstract units of complexity" and then multiplying that number by the developer's coefficient (1x for Alice and 5x for Bob, in the example). Story Points are these "abstract units of complexity". Because they're abstract, we can define Story Points to be any size we like, but conventionally, we define the easiest ticket in the backlog to be one Story Point. That construction allows us to size the rest of our tickets by [Snaking](http://ronlichty.blogspot.com/2014/08/team-estimation.html): sort our tickets, smallest to largest, and then find the first ticket that's about twice as hard as the easiest (the first 2) the first ticket that's about 50% harder than than that (the first 3), etc. The numbers should be difficulty ratios (the easiest "2" should be about twice as hard as the easiest "1"), but we'll restrict our sizes to Fibonacci numbers to save time and sanity.

When new things get added to the backlog, we insert them in the list and infer their size in Story Points.

### How We Convert Them to Estimates

We compute a coefficient for the whole team. First, we track the number of Story Points the team accomplishes each week (our "Velocity," which should be fairly stable as a corollary of the above observation[^corollary]). Then, for a new project, we add up its issues' Story Points and divide by the team's Velocity to get a time estimate.

Isn't this just a complicated way of estimating projects the way we always have? You're breaking a project into pieces, estimating each piece, and then adding them up; isn't that known not to work well? The difference is that Story Points are relative, and Velocity is measured rather than estimated. This yields two big psychological benefits for engineers:
1. If you forget to include testing, code review, etc. in your estimate, that's totally fine. As long as you forget consistently, and the forgotten steps are a fairly consistent proportion of each story, then stories' relative sizes remain the same. The time estimate comes out correct.
1. No one bothers you about deadlines anymore. You're not worried about tomorrow's work at the end of the day, and instead you can just focus on general productivity (our Velocity).

### What About Technical Risk? Early Feedback?

These are both still very important. Big enough risks won't amortize over any reasonable time frame. The solution to these issues is to pick the right milestones, which is orthogonal to the ETA of those milestones. So we'll need to do that too.

[^corollary]: If the ratio of any two team members' completion time is stable, then confounding factors like "my laptop caught on fire this week" are washing out.
