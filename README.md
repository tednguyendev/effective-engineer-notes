# Part 1: Adopt the Right Mindsets

## Focus on High-Leverage Activities

Onboarding and mentoring are two of the highest leverage investments that the author made for the Quora team

Leverage is Impact Produced / Time invested. It is like ROI. Effective engineers are not those who work more, but are those who get more things done in the same amount of time. Leverage is how we can measure the effectiveness of engineers.

Mentoring is a prime example of a high-ROI activity. In a single year, a typical engineer works between 1,880 and 2,820 hours. 5 Devoting even 1 hour every day for the first month (20 hours) to mentor or train a new hire may seem like a large investment; yet it represents only about 1% of the total time the new hire will spend working during her first year. Moreover, that 1% time investment can have an outsized influence on the productivity and effectiveness of the other 99% of work hours.

3 ways to increase leverage:

- By reducing the time it takes to complete a certain activity.
- By increasing the output of a particular activity.
- By shifting to higher-leverage activities.

Don't confuse high-leverage activities with easy wins, however. Building a strong hiring culture wasn't a quick and easy fix; it was a high-leverage activity that required consistent effort over many years.

## Optimize for Learning

People with a fixed mindset believe that "human qualities are carved in stone." They tend to give up early and easily, which enables them to point to a lack of effort rather than a lack of ability as causing failure.

When companies pay you for cushy and unchallenging 9-to-5 jobs, Cohen argues, "what they are actually doing is paying you to accept a much lower intellectual growth rate. When you recognize that intelligence is compounding, the cost of that missing long-term compounding is enormous. They're not giving you the best opportunity of your life. Then a scary thing can happen: … you get complacent and stall."

Mutual funds and bank accounts build your financial capital, but learning builds your human and career capital. You would rather invest your financial assets in accounts that pay high interest rates, not low ones. Why would you treat your time—your most limited asset—any differently?

"If you're offered a seat on a rocket ship, you don't ask what seat. You just get on." That advice to focus on growth served her well: she rose to become a VP at Google, which opened the opportunity for her to later become Facebook's COO.

The solution is to borrow a lesson from Google. Google pioneered an idea called "20% time," where engineers spend the equivalent of one day a week on a side project to make the company better. Initially, 20% time was a controversial proposal; people doubted it would improve the company's bottom line. In fact, the investment empowered engineers to create and launch products like Gmail, Google News, and AdSense—which now comprise three of Google's core offerings.

The former head of Microsoft's Windows division, calls "adjacent disciplines." Knowledge in adjacent disciplines will not only be useful, but you'll also be more likely to retain the information because you'll be actively practicing it.

Moreover, research on learning confirms that the interleaved practice of different skills is more effective than repeated, massed practice of a single skill at preparing people to tackle unfamiliar problems.

After years of observation, Bobby Johnson, a former engineering director at Facebook, concluded that engineering success was highly correlated with "having no fear in jumping into code they didn't know."

Other skills might not translate directly into engineering benefit, but the practice of adopting a growth mindset toward them still makes us better learners and more willing to stretch beyond our comfort zone. This itself is a high-leverage investment.

## Prioritize Regularly

In The Checklist Manifesto, Dr. Atul Gawande shows how the adoption of checklists has drastically reduced errors in field after field, even for the most seasoned experts working on routine tasks. Pilots who follow pre-flight checklists, surgeons who follow operation checklists, and construction managers who follow safety checklists all eliminate large classes of avoidable errors simply by writing steps down and tracking what needs to be done.

Ask yourself on a recurring basis: Is there something else I could be doing that's higher-leverage? If not, continue on your current path. If yes, it's time to rethink what you're doing. The goal isn't to establish a total ordering of all your priorities, since any ordering you make will be based on imperfect information; instead, it's to continuously shift your top priorities toward the ones with the highest leverage, given the information you have.

At the end of the day (or when it comes time for performance reviews), what matters is how much value you've created.

That value is measured in terms of products shipped, users acquired, business metrics moved, or sales made, rather than in terms of hours worked, tasks completed, lines of code written, or meetings attended.

Be wary if you're spending too much time on Quadrant 1's important and urgent activities. A pager duty alert, a high-priority bug, a pressing deadline for a project, or any other type of firefighting all may be important and urgent, but assess whether you're simply addressing the symptoms of the problem and not its underlying cause. Oftentimes, the root cause is an underinvestment in a Quadrant 2 activity.

The act of prioritization is itself a Quadrant 2 activity, one whose importance often gets overlooked because it's rarely urgent.

# Part 2: Execute, Execute, Execute

Just because changes are deployed incrementally, however, doesn't mean that larger features aren't possible or that users see half-finished features. A large feature gets gated behind a configuration flag, which is disabled until the feature is ready.

## Invest in Iteration Speed

In actuality, the worst outage Facebook ever faced over a four-year period lasted only 2.5 hours—much shorter than outages experienced by larger, slower-moving companies. Moving fast doesn't necessarily mean moving recklessly.

Because learning compounds, the sooner you accelerate your iteration speed, the faster your learning rate will be.

faster tools get used more often. If the only option for travel from San Francisco to New York was a week-long train ride, we wouldn't make the trip very often; but since the advent of passenger airlines in the 1950s, people can now make the trip multiple times per year.

faster tools can enable new development workflows that previously weren't possible.

Mayer held occasional office hours, and the teams who got things done were the ones who took advantage of those informal meetings to solicit early and frequent feedback.

Plan ahead. Expend slightly more effort in coordination; it could make a significant dent in your iteration speed. Get the ball rolling on the requirements in your launch checklist, and don't wait until the last minute to schedule necessary reviews.

## Measure What You Want to Improve

"If you can't measure it, you can't improve it."

good metrics help guard against future regressions

In a conversation I had with Sam Schillace, Box's VP of Engineering, he explained a technique called performance ratcheting that they now use to address this problem and apply downward pressure on performance metrics. In mechanics, a ratchet is a device that allows a wheel with many teeth along its edge to rotate in one direction while preventing motion in the opposite direction. At Box, they use metrics to set a threshold that they call a performance ratchet. Any new change that would push latency or other key indicators past the ratchet can't get deployed until it's optimized, or until some other feature is improved by a counterbalancing amount. Moreover, every time the performance team makes a system-level improvement, they lower the ratchet further. The practice ensures that performance trends in the right direction.

just because it's hard to measure a goal doesn't mean that it's not worthwhile to do so. We'll often be faced with tricky situations where intuitively something seems valuable, but it is hard to quantify or takes too much effort to measure.

Focusing on the average response time leads to a very different set of priorities than focusing on the highest 95th or 99th percentile of response times. To decrease the average, you'll focus more on general infrastructure improvements that can shave off milliseconds from all requests. The average is the right metric to use if your goal is to reduce server costs by cutting down aggregate computation time. To decrease the 95th or 99th percentile, however, you'll need to hunt down the worst-case behaviors in your system.

A responsive metric updates quickly enough to give feedback about whether a given change was positive or negative, so that your team can learn where to apply future efforts. Trying to track performance improvements with per-minute response time metrics would be difficult because of their high variance. However, tracking the response times averaged over an hour or a day would make the metric more robust to noise and allow trends to be detected more easily. Responsiveness needs to be balanced with robustness.

"We've generally seen just about everything people throw at databases," explains Percona consultant Baron Schwartz. "Tagging, friends, queues, click tracking, search, paginated displays—we've seen these and dozens of other common patterns done a hundred different ways." As a result, they've internalized useful numbers that they can use to benchmark a particular system's The Effective Engineer performance. They might not know exactly how much better your system might behave with a certain change, but they can compare your performance with expected numbers and let you know what's going well and what has ample room for improvement. In contrast, someone less knowledgeable would need to test various MySQL configurations or architectures and measure what difference (if any) the changes made.

Oftentimes, however, you don't need accurate numbers to make effective decisions; you just need ones that are in the right ballpark. Ensuring you have access to a few useful numbers

## Validate Your Ideas Early and Often

Each email from the Obama campaign was tested on as many as 18 smaller groups, and the best variations often raised 5 to 7x as many donations as the worst one.

An A/B test doesn't just help you decide which variation to launch. Even if you were absolutely convinced that a certain change would improve metrics, an A/B test tells you how much better that variation actually is.

For instance, a large product investment that only yields a 1% lift in retention rates means that you'd likely find more leverage elsewhere, whereas you might decide to double down on the same area had it yielded a 10% improvement.

The lows of a project are more demoralizing when you're working alone. Sand traps that you struggle to get out of, monotonous work that you need to grind through, and bugs that seem to defy all understanding become less draining and more bearable when there's someone there to share your pain.

Similarly, the highs can be less motivating when you're working alone.

## Improve Your Project Estimation Skills

Had we known that the project would have taken 9 months instead of 4, we would've thoroughly explored other alternatives like scoping down the project, doing a more incremental rewrite, or cutting back on other customer obligations.

A more productive approach is to use the estimates to inform project planning, rather than the other way around.

A long estimate is a hiding place for nasty surprises. Treat it as a warning that you haven't thought through the task thoroughly enough to understand what's involved.

Managers challenge estimates, pushing for tasks to be completed sooner. If you've made your estimates granular, however, you can defend them more easily.

Instead of telling a product manager or other stakeholder that we'll finish a feature in 6 weeks, we might instead tell them, "There's a 50% likelihood that we can deliver the feature 4 weeks from now, and a 90% chance that we can deliver it within 8 weeks."

When one hears of disastrous schedule slippage in a project, he imagines that a series of major calamities must have befallen it. Usually, however, the disaster is due to termites, not tornadoes.

Because our team at Ooyala had deferred new feature development for 4 months, when that time budget expired, we suddenly found ourselves hurrying to both complete the player rewrite and address the requests that customers had been patiently waiting for.

Rewrite projects are particularly troublesome for a few reasons:
• They share the same project planning and estimation difficulties as other software projects.
• Because we tend to be familiar with the original version, we typically underestimate rewrite projects more drastically than we would an undertaking in a new area.
• It is easy and tempting to bundle additional improvements into a rewrite.
• When a rewrite is ongoing, any new features or improvements must either be added to the rewritten version (in which case they won't launch until the rewrite completes) or they must be duplicated across the existing version and the new version (in order to get the feature or improvement out sooner).

The fact that your schedule has slipped means that the work in previous months was underestimated. This, in turn, likely means that the entire project was underestimated, including the remaining two months. Moreover, we tend to be much better at estimating the beginnings of projects, where we're working on concrete development tasks that we understand. In contrast, estimating the ends of projects is more difficult; teams often underestimate how long integration takes, and each unexpected issue can throw schedules off by a week or more.

# Part 3: Build Long-Term Value

## Balance Quality with Pragmatism

"Thinking in terms of right and wrong … isn't a very accurate or useful framework for viewing the world … Instead of right and wrong, I prefer to look at things in terms of works and doesn't work. It brings more clarity and is more effective for making decisions."

Good abstractions should be:
• easy to learn
• easy to use even without documentation
• hard to misuse
• sufficiently powerful to satisfy requirements
• easy to extend
• appropriate to the audience

A suite of extensive and automated tests can smooth out the spikes and reduce overall error rates

One engineer finally wrote a basic automated test for a city building, ensuring that an image asset referenced by a building's configuration was actually in the codebase and not deleted mistakenly during a code merge. That simple test started catching a lot of bugs in Cityville's deployments, paying for itself many times over in terms of time saved. When the time savings became obvious, people looked for other strategic tests to help them iterate faster. Writing the first test is often the hardest.

Technical debt doesn't just accumulate when we make quick and dirty workarounds. Whenever we write software without fully understanding the problem space, our first version will likely end up being less cleanly designed than we'd like. Over time, we develop new insights into better ways of doing things. Since our initial understanding of problems always will be incomplete, incurring a little debt is unavoidable; it's just part of getting things done.

## Minimize Operational Burden

During Instagram's early years, Krieger explained, its team consisted of no more than five engineers. That scarcity led to focus. They couldn't afford to engineer any solutions that would break frequently or require constant maintenance. Far and away, the most valuable lesson they learned was to minimize operational burden. Krieger operated like the chief of a small fire department: he knew that each additional feature and new system represented an extra house that the team needed to support—and possibly firefight.

When asked what he'd learned from designing the iPod, Steve Jobs responded, "When you first start off trying to solve a problem, the first solutions you come up with are very complex, and most people stop there. But if you keep going, and live with the problem and peel more layers of the onion off, you can oftentimes arrive at some very elegant and simple solutions. Most people just don't put in the time or energy to get there."

Having too complex of an architecture imposes a maintenance cost in a few ways:
Engineering expertise gets splintered across multiple systems. Every system has its own unique set of properties and failure modes that must be discovered, understood, and mastered.
New engineers face a steeper learning curve
Effort towards improving abstractions, libraries, and tools gets diluted across the different systems.

Suppose we introduce logic into a web server so that if it reads in a misspelled configuration parameter for max_database_connections, it defaults the parameter to 5. The program might start and run as usual, but once deployed to production, we'll be searching everywhere trying to understand why database queries are slower than usual.
Slowly failing systems muddy the sources of code errors, making it difficult for us to discover what went wrong.

Failing fast doesn't necessarily mean crashing your programs for users. You can take a hybrid approach: use fail-fast techniques to surface issues immediately and as close to the actual source of error as possible; and complement them with a global exception handler that reports the error to engineers while failing gracefully to the end user.

Johnson, however, distinguished between two types of automation: automating mechanics and automating decision-making. Automating the mechanics of a sequence of steps tends to be straightforward and testable. Automating the right decisions to make, particularly in the context of building systems that can heal and repair themselves when things go wrong, turns out to be much more challenging.

For example, consider a simple automated rule for a load balancer that handles a failed server by routing traffic destined to that server to others in the group. This policy works great when one server goes down, but what happens if half the servers fail? The policy routes all the traffic destined to those failed servers to the other half. And if the servers had gone down because of too much load, then the automation would end up taking down the entire cluster.

Running batch processes more frequently also allows you to handle assorted glitches transparently. A system check that runs every 5 to 10 minutes might raise spurious alarms because a temporary network glitch causes it to fail, but running the check every 60 seconds and only raising an alarm on consecutive failures dramatically decreases the chances of false positives.

However, even though the cost of failure can be very high, we often don't devote enough resources to developing strategies that address failure scenarios. Simulating failures accurately is difficult
