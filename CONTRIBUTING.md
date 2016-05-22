<!-- https://github.com/nayafia/contributing-template/blob/master/CONTRIBUTING-template.md -->

# Contributing to h11

Thanks for your interest in contributing to h11! Please take a moment
to review this document in order to make the contribution process easy
and effective for everyone involved.

Following these guidelines helps to communicate that you respect the
time of the developers managing and developing this free and open
source project. In return, they should reciprocate that respect in
addressing your issue, assessing changes, and helping you finalize
your pull requests.


## What we're looking for

h11 is largely feature-complete, in the sense that it has a fairly
well-defined scope and (as far as we know) implements pretty much
everything that fits within that scope. If we're wrong, please let us
know :-). But mostly we're not looking for major new features. On the
other hand, the following are all very welcome:

* Bug reports and bug fixes

* API feedback and suggestions, especially based on experience using
  h11

* Help making the docs more clear, complete, and generally useful

* Good examples of using h11 in different settings (e.g. with twisted,
  with asyncio, ...) to accomplish different tasks

* Improvements in test coverage

* Patches that make the code simpler

* Patches that make the code faster


## Contributor responsibilities

* Code should work across all currently supported Python releases.

* Code should follow
  [PEP 8](https://www.python.org/dev/peps/pep-0008/) style. We aren't
  blind sticklers for this though (in fact,
  [not being a blind stickler for PEP 8](https://www.python.org/dev/peps/pep-0008/#a-foolish-consistency-is-the-hobgoblin-of-little-minds)
  is one of the requirements in PEP 8!). If you run pep8 / pycodestyle
  over the code base then it complains about lots of things, but these
  are generally places where "fixing the problem" would make the code
  less readable. Still, though, when in doubt: PEP 8.

* All code changes require at least the addition or fixing of at least
  one test (see below for how to run the test suite). This helps us
  make sure that we won't later accidentally break whatever you just
  fixed, and undo your hard work.

* [Statement and branch coverage](https://codecov.io/gh/njsmith/h11)
  should remain at 100.0%. But don't worry too much -- if you post a
  pull request, then the codecov bot will automatically post a reply
  letting you know whether you've managed this.

* The test suite should pass. The easy way to check is:

  ```
  pip install tox
  tox
  ```

  But note that: (1) this will print slightly misleading coverage
  statistics, because it only shows coverage for individual python
  versions, and there are some lines that are only executed on python
  2 or only executed on python 3, and (2) the full test suite will
  automatically get run when you submit a pull request, so you don't
  need to worry too much about tracking down a version of cpython 3.3
  or whatever just to run the tests.

* Proposed speedups require some profiling and benchmarks to justify
  the change

* Generally each pull request should be self-contained and fix one bug
  or implement one new feature. If you can split it up, then you
  probably should. This makes changes easier to review, and helps us
  merge things as quickly as possible.

* Be welcoming to newcomers and encourage diverse new contributors
  from all backgrounds.

* Respect our
  [code of conduct](https://github.com/njsmith/h11/blob/master/CODE_OF_CONDUCT.md>)
  in all project spaces.


## How to submit a contribution

You don't have to sign a license agreement or anything to contribute
to h11 -- just make your changes and submit a pull request! (Though
you should probably review the
[MIT license we use](https://github.com/njsmith/h11/blob/master/LICENSE.txt)
and make sure you're happy licensing your contribution under those
terms.)

If you're new to Github and pull requests, then are some tutorials on
how to get started:

* [Make a pull request](http://makeapullrequest.com/)

* [How to contribute to an Open Source Project on GitHub](https://egghead.io/series/how-to-contribute-to-an-open-source-project-on-github)


## After you submit a PR

We'll try to review it promptly and give feedback -- but if you
haven't heard from us after a week, please do send a ping! It's
totally fine and normal to post a comment that just says "ping".

If your PR needs further changes before it can be merged, just make
more changes in your branch and push them to Github -- Github will
automatically add your new commits to the existing PR. But Github
*won't* automatically *tell* anyone that new commits have been added,
so after you've fixed things and are ready for people to take another
look, then please post a comment saying so! That will send us a
notification so we know to take another look.

## And again, thanks!