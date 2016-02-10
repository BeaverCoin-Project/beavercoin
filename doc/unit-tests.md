<<<<<<< HEAD
Compiling/running beavercoind unit tests
------------------------------------

beavercoind unit tests are in the `src/test/` directory; they
use the Boost::Test unit-testing framework.
=======
Compiling/running unit tests
------------------------------------

Unit tests will be automatically compiled if dependencies were met in configure
and tests weren't explicitly disabled.
>>>>>>> pr/5

After configuring, they can be run with 'make check'.

<<<<<<< HEAD
	cd src
	make -f makefile.unix test_beavercoin  # Replace makefile.unix if you're not on unix
	./test_beavercoin   # Runs the unit tests
=======
To run the bitcoind tests manually, launch src/test/test_bitcoin .
>>>>>>> pr/5

To add more bitcoind tests, add `BOOST_AUTO_TEST_CASE` functions to the existing
.cpp files in the test/ directory or add new .cpp files that
<<<<<<< HEAD
implement new BOOST_AUTO_TEST_SUITE sections (the makefiles are
set up to add test/*.cpp to test_beavercoin automatically).


Compiling/running BeaverCoin-Qt unit tests
---------------------------------------

Bitcoin-Qt unit tests are in the src/qt/test/ directory; they
use the Qt unit-testing framework.

To compile and run the tests:

	qmake bitcoin-qt.pro BITCOIN_QT_TEST=1
	make
	./beavercoin-qt_test
=======
implement new BOOST_AUTO_TEST_SUITE sections.

To run the bitcoin-qt tests manually, launch src/qt/test/bitcoin-qt_test
>>>>>>> pr/5

To add more bitcoin-qt tests, add them to the `src/qt/test/` directory and
the `src/qt/test/test_main.cpp` file.
