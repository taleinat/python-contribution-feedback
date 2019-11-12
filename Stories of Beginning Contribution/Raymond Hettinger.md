* Author: Raymond Hettinger
* Date: Aug. 9th, 2019
* Posted on: [core-mentorship mailing list](https://mail.python.org/archives/list/core-mentorship@python.org/message/JKIE5ZMML3Y66RLWPSSPLJ7HKSBZ3PPZ/)

---

In the late 1990's, I learned about Python from a classmate during a
Matlab training course and took it back to my company (a large insurance
corp) where I started replacing Perl and Awk with Python.  In 2000, I
started studying C source and reading posts in the comp.lang.python
newsgroup and on the developer mailing list. I participated in early
discussions about iterators and was one of the folks who nudged GvR to
let dict iteration default to key-by-key instead of item-by-item.
Unpersuasively, I argued that "in" should have the same meaning in "for
k in d" as it does in "k in d".  But I did find traction when citing my
AWK experience (which also loops key-by-key) and my SETL experience
where Python looping key-by-key would naturally support set operations. 
In the end, GvR decided to go with looping over keys instead of items
and I had my first little victory -- I had had some influence over a
core language feature. The only reward for that effort was that t  
 he next release of Python was more expressive and fun to use.  In all
other respects, the "contribution" was doomed to oblivion. Afterwards, I
submitted a few of minor issues most of which were rejected
immediately.  Only the dict.pop() suggestion was accepted.  
  
When iterators landed in Python, I became fascinated (perhaps even
obsessed) because they opened the door to capabilities I had had in
other languages (OCAML, APL, Smalltalk).  So in 2002 my first
substantive contribution was suggesting that enumerate() be added as
builtin.  Because I had fecklessly participated in C++ standardization a
decade earlier, I was not surprised by how involved the effort was:
writing a PEP, interminable discussions about what to name it, and that
the process took a couple months even after the PEP was written.  
  
The environment was intimidating. I was awestruck by giants like GvR,
Fredrik Lundh, Tim Peters, and Alex Martelli -- not awestruck because of
their stature but rather because of their intellectual depth and
accomplishments. And even though some of them were very sharp with me,
it was an honor just to sit at the table and learn from them.  There
were also folks who had very strong opinions about top-posting and how
you worded email (i.e. invisible cultural rules, thorns, and snares at
every turn).  
  
One important early lesson was that my years of writing locally
distributed applications didn't translate easily to a widely used
general purpose tool.  At first, I felt like any code change I proposed
would be answered 15 minutes later by Tim Peters who would explain why
my change would break or impair some AS400 or Cray System or would
interact poorly with some OS that I had never heard of.  I have been
programming in C for 15+ years, but only when I came to Python did I
learn how little I knew about language guarantees (or lack thereof),
race conditions, reentrancy, and weird OS interactions. The Python C API
was just awful to program with -- it took a good while learn to write
code that didn't leak or have reentrancy problems (annoyingly, a DECREF
can trigger arbitrary code execution).  The world was much more complex
than I had imagined.  
  
Somewhere in 2002, I was given commit privileges.  There was no
fanfare.  I was heavily supervised and didn't have any extra weight in
discussions.  At the time, we didn't use the term "core developer", so
it didn't feel special at all. Of late, I think it was a mistake to
adopt to term at all.  The term makes it feel like an honor that is
selectively granted to a privileged few. Instead, it might be better to
call it "code janitor" because most of the work of core development is
thankless and janitorial. When I was given admin rights on the tracker
and the repo, it wasn't an honor of any sort -- it was just volunteering
to shoulder some of the infrastructure maintenance.  
  
At the time, Fred Drake was the gatekeeper for the Python docs. Nothing
changed without going through him and he was a stickler about following
a style guide (we write "for example" instead of "e.g.").  Because I had
had a tech writing background, eventually, he granted me the ability to
work on the docs more extensively.  But the door was only part way open,
I still had to wrestle with the TeX markup, made doubly difficult
because I couldn't figure-out how to get the docs to build on Windows. 
A lesson here is that tooling can be a barrier to contribution (even
now, "all you have to do" is learn to use git, use GitHub, read the dev
guide, learn unittest and its test support tools, install Sphinx in a
virtual environment, learn reST markup, install and run blurb, run make
patch check and make TAGS, learn the argument clinic, learn the C API,
make a debug build, drill into nested macros, run a C debugger,
figure-out how to test for refleaks, cope with the social environment,
learn to  
 use the tracker, follow a bunch of mailing lists, use discuss, user
perf, etc.).  
  
That's my early contribution story.  However, I should mention that some
of these early challenges aren't just beginner issues, some never go
away.  When we switched to git and Github, I stopped contributing for
six months until Ned Deily helped me with the new tooling.  There are
new invisible social rules (being accused of a code-of-conduct violation
for describing a test as "fragile" when it relied on non-guaranteed
implementation details).  The "simple change" of adding a comma for a
thousand's separator took months and ate nearly a hundred hours for PEP
research, writing, and subsequent discussions.  Even now, I have a hard
time convincing other devs that we had a 20% performance degradation in
3000+ functions (it's fixed now) or that spewing syntax warnings that
user can't control will lead to an unfavorable user experience.  Even
now, as a trigager, I can find severe problems in submitted patch and
have those comments dismissed by senior devs who happen to work at the
same com  
 pany as the patch submitter. There are some patch reviewers who can eat
a lot of your time, making it cost prohibitive to participate.  
  
In short, the Python core development world is populated by humans,
humans who have human weaknesses, humans who can be tribal, humans who
have perceived friends and enemies, human who having differing
viewpoints, cultural values, and skillsets, humans who have limited time
and resources, humans whose only commonality is that they care about
Python programming language.  
  
  
Raymond  
  
  
P.S.  One other thought relevant to this discussion is that lack of
money can also be a barrier to participation. When I started, I didn't
have money for decent computer. It had an exposed motherboard and a
jury-rigged cooling plate so that it wouldn't overheat during a build. 
I had to pay $500 for a Microsoft compiler just to build Python.  Last
year, I was reminded of this when I learned that one of our more active
devs was also working with inadequate tooling and we had to ask the PSF
to buy him a computer. In a similar vein, for the self-employed, it can
be very expensive to take a week off to attend a sprint.  There are
monetary costs to participation.  
  
P.P.S. When I started, there was no notion of mentorship.  It was mostly
sink-or-swim.  That said, Alex Martelli and Tim Peters did invest time
in helping me develop my skills.  Without them, I wouldn't be here
today.  Thank you both :-)

One other thought on barriers to participation:  When I started, being a
Windows user in Linux world was crippling.  Tim Peters helped me
overcome PuTTY setup issues; however, my \*nix experience was somewhat
dated and a lot of the CPython world was Linux centric.
