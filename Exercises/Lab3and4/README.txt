This project implements a multi-component C++ application designed to process numerical data stored as pairs of (x, y) values. The program reads the dataset, performs various mathematical analyses, and outputs the results to separate text files. A strong emphasis is placed on modular design, with functionality split across dedicated source files.
Project Structure

The program is divided into three source files, each handling a distinct responsibility within the application:

1. AnalyseData.cxx

This is the central driver of the program. Its main tasks include:

Opening and reading the input file data.txt

Storing x–y pairs into two vectors

Presenting an interactive menu to the user

Calling analysis functions that reside in a separate module

Handling basic user input and program flow
Files Included
AnalyseData.cxx

Contains the program’s main() function.

Loads (x, y) values from data.txt into vectors.

Shows a menu allowing the user to choose which operation to run.

Uses the functions declared in CustomFunctions.h and implemented in CustomFunctions.cxx.

CustomFunctions.cxx

Implements all analysis routines, including:

Displaying the first N rows of the dataset.

Computing magnitudes of the vector pairs.

Performing a straight-line least-squares fit and evaluating the residual sum.

Computing  x to the power of y using exp(y * log(x)) instead of loops or pow().

Calculating the magnitude of user input using a template function.

CustomFunctions.h

Provides the function declarations used by the main program.

Ensures the task functions can be called from AnalyseData.cxx.




