# detect-large-text-encoding
Detects or guesses the encoding of large given texts. For some encodings the library provides a safe result, for othes the result is a best guess.
The library is especially designed for (very) large text files. Many GB are not a problem and in many cases this also takes only a few (milli-)seconds. Nevertheless, for some encodings a statistical analysis is required, this causes a longer computation time in these cases for good results.
