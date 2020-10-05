This document is a subjective collection of takeaways from about 15 stories about beginning contribution to Python. These stories were submitted during September and October 2019.

# Main Issues

These are things which came up repeatedly in the stories, or that otherwise especially stood out.

## Slow/No Responsiveness

Very slow responses to new contributors are common. These often cause the contributors to feel ignored, marginalized. These also sometimes feel like failures on their part.

The opposite is also true: Getting attention, and having your suggestions taken seriously by core devs, results in very positive feelings and reactions.

### Quotes

> I raised the issue on some other Python mailing list (I forget which one), caught the attention of Guido who showed some real willingness to listen to the argument. (André Roberge)

> when you are perceived as a "nobody", even if you write code that solves an issue, too many core developers find it easy to completely ignore you on the bug tracker (André Roberge)

> The only difficulty I believe is the lack of reviews on the pull requests. (Sanyam Khurana)

> Pushed it and asked for review. And then nothing anymore ... (Anonymous)

## Long, slow process

Even when things do get some attention, progress and are eventually resolved, this often takes years.

### Quotes

> Eventually everything got merged but it look almost 3 years for a really simple and obvious bugfix. (Jeroen Demeyer)

> I found that spending 6 months or more on a single PR was a bit too much for me. (Jonathan Gossage)

> Initially, the person has studied parts of code that were essential to fix a bug, but till the time a review comes in, they might have to re-read what they wrote and what is already there in order to make changes. While it doesn't happen always, but it is quite common (at least for me and few people I helped to contribute). (Sanyam Khurana)

> It was right before the feature freeze for 3.6, and the reviewer
wanted more time to think about design issues.  Then after the release
he appeared briefly before disappearing for a while (and never replied
to my last message) and then I got busy too and forgot about it (Stephen J. Turnbull)

> I hit a bug while working with msilib, which let me to a 10 year old open ticket (at the time). The issue already had a patch attached, core developers seemed to like it, but felt it should also address an (only loosely related IMO) memory issue. I took the patch and created a PR, and also addressed the memory issue. Nothing. Finally Steve Dower discovered the PR and merged it another two years later. (Tzu-ping Chung)

> Is there anything I should do about the PR, or it just got lost into the void? (Tymoteusz Wołodźko, comment on his PR [GH-16813](https://github.com/python/cpython/pull/16813))

## Where to start?

Many would-be contributors have trouble finding good places to begin contributing.

### Quotes

> I’m still interested and have the objective to become a contributor, but I am faced with the question of where to start. (Lee Congdon)

> Went trough the 'easy' issues but are not easy at all or very discussed. So probably the real easy ones are gone. Tried to test some patches and found a few new ones appearing that I could have solved but then got answers from core-devs that it was not good. Somehow they don't want to fix/adjust things in the libraries because it brings down the speed of the function or doesn't follow the official protocol. (Anonymous)

## Mentorship Helps

Many contributors thank those who actively helped them when they were getting started.

### Quotes

> When I started, there was no notion of mentorship.  It was mostly sink-or-swim.  That said, Alex Martelli and Tim Peters did invest time in helping me develop my skills.  Without them, I wouldn't be here today.  Thank you both :-) (Raymond Hettinger)

> Nick Coghlan came to India for PyCon Pune and helped a lot of folks during sprints with setting up the dev environment and filtering down bugs. Having someone who is already experienced with the workflow helped everyone in kickstarting their contributions. (Sanyam Khurana)

> My initial stab at poking around CPython first issues a few years ago just left me confused and since then I have had a chance to revisit that since I was lucky enough to have a mentor who sat down with me in person and very patiently explained to me how to go about it. (Sushma)

> The same people (i.e., the core developers) were reviewing the code and discussing the feature on the Bug tracker. Also, they were infinitely patient on the IRC as well as in the reviews. Most crucially, one of the core-devs made a judgement call to accept the change in the face of weak-consensus.

## A Lot to Learn to Get Started

### Quotes

> even now, "all you have to do" is learn to use git, use GitHub, read the dev guide, learn unittest and its test support tools, install Sphinx in a virtual environment, learn reST markup, install and run blurb, run make patch check and make TAGS, learn the argument clinic, learn the C API, make a debug build, drill into nested macros, run a C debugger, figure-out how to test for refleaks, cope with the social environment, learn to
 use the tracker, follow a bunch of mailing lists, use discuss, user perf, etc. (Raymond Hettinger)

> I already had some experience with contributing to Mozilla's Gecko engine and marionette, so while I didn't find it hard to know how to accomplish a search or understand the meaning of fields, I still couldn't understand a few terms -- for example -- what a "nosy list" means. (Sanyam Khurana)

> I came with some experience of contributing to OSS already. I had at least a passing familiarity with the underlying tech (GitHub, make, testing, C, RST, Valgrind, etc.), knew about the IRC channels, and had some time. (Utkarsh Upadhyay)

> Sweating, double checking, more and more tabs in the browser go open to read. (Anonymous)


## It's Intimidating

> I was very afraid (impostor syndrome) initially and just wanted to at the least understand the workflow for contributing to CPython during 2 days of the sprint. Landing a patch was very far from what I'd imagine in my wildest dreams. (Sanyam Khurana)

> I realized I was very hesitant to say much initially, but I just needed to get out of my own way and ask for help/not overthink too much, even on the what I presumed to be the basic things. (Sushma)

> Many months pass by, and it keeps spooking in my head, that somehow my understanding of the library is not that bad and this stupid small feature could be contributed to Python. Still, intimidated by all those great developers, it seems one giant leap. (Anonymous)


# Other Notes

Beginning contribution today is easier than it used to be, but there is still a lot to improve.

Using b.p.o. is often a very significant hurdle.

First-time contribution is incredibly hard: It's intimidating, there are a lot of tools to learn, bugs.python.org makes things harder, and there is a LOT to read. **After going through all of that, having your contribution ignored is incredibly deflating.** I have a feeling that this is especially true for potentially great contributors, who follow all of the rules and suggestions and spend many hours before their first patch/PR.
