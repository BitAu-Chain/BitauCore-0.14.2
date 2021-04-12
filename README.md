BitAU Core integration/staging tree
=====================================

https://bitau.co

For an immediately usable, binary version of the BitAU Core software, see
https://bitau.co/en.

Further information about BitAU Core is available in the [doc folder](/doc).

What is BitAU?
----------------

BitAU is a free open source project that was created by a small group of Bitcoin
enthusiasts from diverse backgrounds. In contrast to the other prominent Bitcoin
forks, BitAU was specifically designed from the beginning to inspire innovation in the
Bitcoin ecosystem and give value to the vision of decentralization. Whereas the others
were born from hostility and an ambition to dominate, BitAU arises from a desire to
protect Bitcoin and ensure that it not only maintains its position as the dominant
cryptocurrency but continues to grow until its liberating roots stretch deep into the
economic life of all nations.

For more information read the original BitAU whitepaper.

License
-------

BitAU Core is released under the terms of the MIT license. See [COPYING](COPYING) for more
information or see https://opensource.org/licenses/MIT.

Development Process
-------------------

The `master` branch is regularly built (see `doc/build-*.md` for instructions) and tested, but it is not guaranteed to be
completely stable. [Tags](https://github.com/BitAu-Chain/BitAU/tags) are created
regularly from release branches to indicate new official, stable release versions of BitAU Core.

The https://github.com/BitAu-Chain/gui repository is used exclusively for the
development of the GUI. Its master branch is identical in all monotree
repositories. Release branches and tags do not exist, so please do not fork
that repository unless it is for development reasons.

The contribution workflow is described in [CONTRIBUTING.md](CONTRIBUTING.md)
and useful hints for developers can be found in [doc/developer-notes.md](doc/developer-notes.md).

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test on short notice. Please be patient and help out by testing
other people's pull requests, and remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write [unit tests](src/test/README.md) for new code, and to
submit new unit tests for old code. Unit tests can be compiled and run
(assuming they weren't disabled in configure) with: `make check`. Further details on running
and extending unit tests can be found in [/src/test/README.md](/src/test/README.md).


The CI (Continuous Integration) systems make sure that every pull request is built for Windows, Linux, and macOS,
and that unit/sanity tests are run automatically.

### Manual Quality Assurance (QA) Testing

Changes should be tested by somebody other than the developer who wrote the
code. This is especially important for large or high-risk changes. It is useful
to add a test plan to the pull request description if testing the changes is
not straightforward.
