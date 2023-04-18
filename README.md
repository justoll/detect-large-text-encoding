# detect-large-text-encoding
Detects or guesses the encoding of large given texts. For some encodings the library provides a safe result, for othes the result is a best guess.

The library is especially designed for (very) large text files. Many GB are not a problem and in many cases this also takes only a few (milli-)seconds. Nevertheless, for some encodings a statistical analysis is required, this causes a longer computation time in these cases for good results.

This Library is also resilient to isolated encoding errors or small areas of deviating encoding. 




----- Linux  -----

You need the tool "enca" installed from https://github.com/nijel/enca. Install it with

    ./configure
    make 
    make check
    make install

Then continue with installation of this tool:

    sudo ldconfig
    [add line] /usr/local/lib
    make clean
    make 
    make install

-> installs .so file to /usr/local/lib
