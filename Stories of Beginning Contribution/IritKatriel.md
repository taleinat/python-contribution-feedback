* Author: Irit Katriel
* Date: Oct. 18th, 2020
* Posted on: [GitHub PR](https://github.com/taleinat/python-contribution-feedback/pull/1)

---

My first checkout of the cpython codebase was in order to debug a segfault due to a GC 
trashcan related bug in python 3.8 (bpo-40608). Fortunately, this was caught by a unit
test one of my colleagues put in a few years ago due to a bug that impacted us while we
were using Python 2.6 (bpo-16602). It was hard enough to debug the unit test during 
migration from 3.7 to 3.8, and I would not have wanted to deal with this as a prod issue
under time pressure!

The issue was that new trashcan macros were introduced, but the old ones remained for
backwards compatibility yet were no longer working correctly in all cases. The fix for
us was to move to use the new macros, so we don't have a problem with this anymore. 
However, I would have had a much easier time if the old macros were just removed and 
I was forced by a compiler error to use the new ones. The issue I reported is still 
open, and people migrating to Python 3.8 might still have the problems I faced.

After that initial contribution, I got a taste for working on cpython and started
looking around for interesting things to do, with the blessing and support of my
employer. I contributed a few localised bugfixes and doc updates (a couple of bugs I
found but mostly from open tickets). Some of them were merged very quickly and some are
still open. Vinay is particularly responsive re contributions to the logging library,
while the other extreme is pdb where the response to submitting a PR can be anything
from silence to core devs removing themselves from the nosy list.

I have been learning a lot about the cpython codebase and dev processes from discussions
in tickets and PRs (Serhiy and Raymond in particular have given me a lot of their time,
but many others have also been very patient and helpful). I still have a lot to learn,
of course.

This is my first time getting involved with a large open source project . In comparison 
to dev teams I worked in at various companies, my impression is that this is a very open,
friendly and accepting team. On the other hand, due to the voluntary nature of the team,
it seems that different parts of the codebase enjoy very different levels of care, and
I wonder whether it makes sense to trim down the standard library to a smaller set which
is maintained to a higher standard (for example - should pdb be dropped or should the
bugs in it be fixed? And if no core dev has an interest in that, how will it happen?).

Another point I was wondering about is how to get more PR reviewing going on among 
non-core contributors. The PR backlog is a well known pain point, and I think that
new contributors can learn a lot from getting involved in this work. I don't know
quite how to encourage it though.

Thank you, Tal, for soliciting my input. 
