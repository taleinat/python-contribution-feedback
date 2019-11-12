* Author: Utkarsh Upadhyay
* Date: Aug. 2nd, 2019
* Posted on: [core-mentorship mailing list](https://mail.python.org/archives/list/core-mentorship@python.org/message/DC6IQ2PT7NKFANU45RTSRIIS3AVTI55V/)

---

Mine is a successful contribution story:
http://blog.musicallyut.in/2017/09/07/my-first-commit-in-python.html

It came close to not being one, though: my PR holds the dubious
distinction of being the first to be rolled back under the then-newly
created Buildbot policy of reverting first and asking questions later.

The key things which made the contribution successful were:

- I came with some experience of contributing to OSS already. I had at
least a passing familiarity with the underlying tech (GitHub, make,
testing, C, RST, Valgrind, etc.), knew about the IRC channels, and had
some time.

- The change was relatively small (even though it came with some
history with people on both sides of the debate and it ended up sparking
off a few other bug fixes).

- The same people (i.e., the core developers) were reviewing the code
and discussing the feature on the Bug tracker. Also, they were
infinitely patient on the IRC as well as in the reviews.

- Most crucially, one of the core-devs made a judgement call to accept
the change in the face of weak-consensus.

My 2 cents about the process: 

- The discussion got a bit difficult to follow at times
(https://bugs.python.org/issue30302), even for me, and I had to
repeatedly cross-reference and rephrase/copy arguments just to keep
everything clear for myself.

  TBH, I was quite impressed that Victor was able to summarize the 3
month-long thread (interspersed with code-review and musings), create a
summary, and make a decision. 

  Maybe it would be a good idea to keep the bug-tracker exclusively for
feature/bug level discussion and keep all code-related discussion on
GitHub?

  Are there people who are still attaching patches instead of making PRs? 

- Though nosy list was populated for the issue, I was a bit rudderless
in which suggestions on the thread to heed to and which required more
discussion. 

  Hence, I ended up making changes to the PR with almost every comment on
the issue until Victor told me to slow down and to let the discussion on
the issue play out because not all suggestions will make it to the PR,
or at least not necessarily this PR.

  So, Victor helpfully mentored me through the contribution through a chat
on the IRC about half-way through the thread; this was separate from
code-reviewing and feature discussion.

  Though I may be wrong here, I do not think I was the odd-ball who came
with a bug and a fix and was mentored post-fact.

  Perhaps when such a drive-by contribution comes in and is sufficiently
interesting for one of the core-devs, the dev can pro-actively become
the "mentor" early on in the thread?
