Sources: [Write More Tests, Part 1](https://writemoretests.com/2012/02/how-to-estimate-like-adult-part-1.html), [Part 2](https://writemoretests.com/2012/02/estimating-like-an-adult-what-to-steal-from-agile.html), [An Epic Treatise on Scheduling, Bug Tracking, and Triage](https://apenwarr.ca/log/20171213)

### Observation

If Staff Engineer Alice takes a day to implement a feature that would have required a week from Junior Engineer Bob, then that 5x ratio generalizes to other projects. Bob will typically take 5x as long to implement a feature as Alice would[^claim]. Story Points follow naturally.

### How Story Points Follow

Given the observation above, it would make sense to estimate project duration by first estimating project size in "abstract units of complexity" and then multiplying that estimate by the implementing developer's coefficient (1x for Alice and 5x for Bob, in the example). Story Points are these "abstract units of complexity".

### How Do We Use Them?

In Agile, you compute a coefficient for the whole team. You track the number of Story Points the team accomplishes each week (their "Velocity," which should be fairly stable as a corollary of the above observation[^corollary]). For a new project, you add up its stories and divide by the team's Velocity to get a time estimate.

Isn't this just a complicated way of estimating projects the way we always have? You're breaking a project into pieces, estimating each piece, and then adding them up; isn't that known not to work well? The difference is that Story Points are relative, and Velocity is measured rather than estimated. This yields two big psychological benefits for engineers:
1. If you forget to include testing, code review, etc. in your estimate, that's totally fine. As long as you forget consistently, it just means your team's Velocity is slightly lower, and the time estimate comes out correct.
1. No one bothers you about deadlines anymore. You're not worried about tomorrow's work at the end of the day, and instead you can just focus on general productivity.

### How Do You Estimate Story Points?

[Snaking](http://ronlichty.blogspot.com/2014/08/team-estimation.html): You sort your stories, smallest to largest, and then figure out the cutoffs between the 1s, the 2s, the 3s, the 5s, etc. The numbers should be difficulty ratios (the easiest "2" should be about twice as hard as the easiest "1"), but you restrict yourselves to fibonacci numbers to save time and sanity.

When new things get added to the backlog, you insert them in the list.

### What About Technical Risk? Early Feedback?

These are both still very important. In aggregate, they affect the team's velocity (for big enough risks, they won't amortize over any reasonable time frame, and you'll just miss your deadline). The solution to these issues is to pick the right milestones, which is orthogonal to the ETA of those milestones. So we'll need to do that too.

[^claim]: This is an empirical claim; the evidence I've seen to support it is the endorsement of Avery, the "Write More Tests" person, and the prior experience of a few people at Pachyderm (who I'll name once I have their permission).

[^corollary]: If the ratio of any two team members' completion time is stable, then confounding factors like "my laptop caught on fire this week" are washing out.
