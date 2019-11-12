* Author: Stephen J. Turnbull
* Date: Aug. 1st, 2019
* Posted on: [core-mentorship mailing list](https://mail.python.org/archives/list/core-mentorship@python.org/message/QUFWPITZUSG5TMNFHBWT7YZUD75DRBMH/)

---

First I should say I'm a bit of an odd fish; I've been participating  
in Python development in one way or another for about 15 years, and  
included as an author on 2 PEPs (other contributors were the  
proponents who handled the actual submissions), though I've never made  
a direct code contribution to CPython.  So I don't know that my  
stories will be very useful to "typical" new contributors.  
  
# Story \#1
  
A couple of years ago I tried to contribute an enhancement to the  
zipfile module, which would add the ability to set the file name  
encoding when reading a zip file to both the ZipFile class and to the  
convenience command line interface.  (There are workarounds for the  
zipfile module, but they're not pretty or obvious to users.)  For  
details see issue 28080 on bpo.  
  
It was right before the feature freeze for 3.6, and the reviewer  
wanted more time to think about design issues.  Then after the release  
he appeared briefly before disappearing for a while (and never replied  
to my last message) and then I got busy too and forgot about it (the  
need for the feature used to come in spates at certain times of year,  
which mostly coincide with feature freeze ;-).

This doesn't bother me, I know how that stuff goes, and as far as I'm  
concerned, it's a problem that's solving itself, because fewer and  
fewer people I correspond with are using the legacy utilities that  
create zipfile with filenames encoded in Shift JIS.  I still see them  
once in a while but nowhere near as often as when I wrote that patch.  

A quick search on zipfile in bpo suggests that nobody has followed up  
on that issue or posted a duplicate, so maybe everybody else feels the  
same way.  I guess I should think about closing it, or maybe pinging  
the committers who showed an interest.  

# Story \#2  

Last year somebody on Python-Ideas said that there didn't seem to be a  
description of the requirements to get a PEP approved for publication  
(vs accepted for implementation).  
  
So I directly wrote up a PR (the material needed was mostly already  
there, but in a different section), and after a day or three of  
discussion, it got committed pretty much immediately.  (Pull request  
\#789.)
