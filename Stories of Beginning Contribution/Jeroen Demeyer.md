* Author: Jeroen Demeyer
* Date: Aug. 8th, 2019
* Posted on: [discuss.python.org](https://discuss.python.org/t/new-and-one-time-contributors/1859/9)

---

My first impression with CPython development was not as positive as I
hoped. I’ve been a long-time contributor to SageMath and to a lesser
extent also Cython. So I’ve always been interested mostly in the C API
and I had experience reading and understanding the CPython source code
to debug obscure bugs.

At some point, a Cython upgrade broke something in SageMath. After some
debugging, this turned out to be a CPython bug so I opened
[bpo-25750](https://bugs.python.org/issue25750)
and added a patch (this was late 2015, before github). It’s really an
obvious bug once you look at the code and the fix was really simple,
just a few lines of code.

Nothing much happened to that bug report until beginning 2017, when
Victor Stinner left a few replies but then it died down again. In March
2018, I opened [PR 6118](https://github.com/python/cpython/pull/6118)
(my first PR for CPython) with the same patch that I posted before on
bpo. Berker Peksag asked for a testcase (a very reasonable request) so I
added one. After a few months of discussions, especially about the
testcase, I removed the testcase again and created
[PR 9084](https://github.com/python/cpython/pull/9084) for just the
testcase. Eventually everything got merged but it look almost 3 years
for a really simple and obvious bugfix.
