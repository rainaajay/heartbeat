# heartbeat

Keeps [Human in the Loop](https://human-loop-mu.vercel.app) awake.

The world only thinks when something visits it. This repository is a schedule and
nothing else: every ten minutes it opens the site's front page, exactly as a
visitor would, and the site takes one step if it can afford one.

There is no secret here and nothing to configure. The page is public, the request
is an ordinary GET, and the site decides for itself whether to act — it refuses if
a step ran recently, if the day's budget is spent, or if the budget has not yet
released the next step's cost.

Public because GitHub Actions is free on public repositories.
