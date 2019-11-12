* Author: André Roberge
* Date: Aug. 1st, 2019
* Posted on: Private email

---

My only success I wish to comment upon: In the 2 to 3 transitions, Guido
had thought to remove both raw\_input and input. Educators discussing on
the edu-sig mailing list saw this as really counterproductive when it
came to teaching Python to beginners. Taking a clue from those
discussions, I raised the issue on some other Python mailing list (I
forget which one), caught the attention of Guido who showed some real
willingness to listen to the argument.  This lead me to write
[a PEP](https://www.python.org/dev/peps/pep-3111/) in 2006 which was
accepted and reversed partly the original plan.

**Takeaway:** it makes a big difference when core developers listen to, and
are willing to consider contributions from outsiders.

---

# First failure

In 2011, [an issue](https://bugs.python.org/issue10716)
was created to modernize Pydoc.

In 2015, I created a small project on Github to address the original
issue (and did a bit more) and submitted the idea
[to the bug tracker](https://bugs.python.org/msg234936). After getting
feedback from one user, I restricted the changes I made so as to only
address the original bug report. This went nowhere.  If you read the
discussion on the bug tracker, you will find that, later, some
discussions took place (in 2016) in a separate location (core-membership
mailing list), without prior warning.  No one ever said anything about
my code not "solving" the original issue ...  Since then, apparently,
someone has very recently created a patch from my original code but it
is still awaiting a review.

A few days ago, I got
[a request](https://github.com/aroberge/mod_pydoc/issues/4) from the
Spyder IDE folks to add a license as they are apparently interested in
using my code (see the last comment on
[the issue](https://github.com/spyder-ide/spyder/issues/9696). So, at
least someone will get the benefit.

**Takeaway:** when you are perceived as a "nobody", even if you write code
that solves an issue, too many core developers find it easy to
completely ignore you on the bug tracker.

---

# Second failure

In 2015, a bug in the turtle module was reported on
[the edu-sig list](https://mail.python.org/pipermail/edu-sig/2015-March/011207.html).
I took the time to check it, and wrote the code require to fix it,
submitting everything to
[the bug tracker](https://bugs.python.org/issue23660). This was
completely ignored until 2018 where it was tentatively closed. In the
discussion, it was mentioned that "this would impact existing teaching
material already published" which, in my opinion, is nonsense as using
the parameters that were "buggy" would only create confusion for
students, so that no instructor in their right mind would use it.

**Takeaway:** same as before.

---

# Summary of the important points of the two "failures"
 
In both instances, code was submitted that addressed an issue (one
filed by a core developer, another by me on behalf of someone else).
This code (and its "output") appeared to never have been even looked
at by anyone in a position to do a commit, nor was any feedback given
by them.

---

I do understand that everyone is a volunteer, and that there isn't
enough time to address every issue.  But when I saw a discussion on
modernizing Pydoc continuing after I submitted code to address the
original issue, discussion which completely ignore my code, it left a
rather sour taste in my mouth.
