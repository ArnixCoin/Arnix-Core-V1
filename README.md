Official WebSite
================================

https://www.arnixproject.com



What is Arnix?
----------------
<img src="https://avatars1.githubusercontent.com/u/35616636?s=400&u=8d569d78b202e54e6fa06554274e0419a0468103&v=4" alt="ArnixCoin" >

Arnix is a lite version of Bitcoin using scrypt as a proof-of-work algorithm.
 - 2.5 minute block targets
 - subsidy halves in 840k blocks (~4 years)             
 - ~200 Million total coins

The rest is the same as Bitcoin.
 - 50 coins per block
 

For more information, as well as an immediately useable, binary version of
the Arnix client sofware, see https://www.arnixproject.com.


WhitePaper
----------------
https://arnixproject.com/whitepaper.pdf


License
-------

Arnix is released under the terms of the MIT license. See `COPYING` for more
information or see http://opensource.org/licenses/MIT.

Development process
-------------------

Developers work in their own trees, then submit pull requests when they think
their feature or bug fix is ready.

If it is a simple/trivial/non-controversial change, then one of the Arnix
development team members simply pulls it.

If it is a *more complicated or potentially controversial* change, then the patch
submitter will be asked to start a discussion with the devs and community.

The patch will be accepted if there is broad consensus that it is a good thing.
Developers should expect to rework and resubmit patches if the code doesn't
match the project's coding conventions (see `doc/coding.txt`) or are
controversial.

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/arnix-project/arnix/tags) are created
regularly to indicate new official, stable release versions of Arnix.

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test. Please be patient and help out, and
remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write unit tests for new code, and to
submit new unit tests for old code.

Unit tests for the core code are in `src/test/`. To compile and run them:

    cd src; make -f makefile.unix test

Unit tests for the GUI code are in `src/qt/test/`. To compile and run them:

    qmake BITCOIN_QT_TEST=1 -o Makefile.test bitcoin-qt.pro
    make -f Makefile.test
    ./arnix-qt_test
 
