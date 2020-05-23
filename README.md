# Hommel-s-adjustment-binaries
This repository contains the binaries (Windows and Linux) of the program Hommel, a program to calculate Hommel's adjustment

This program calculates and saves the following values in case of multiple comparisons, according to Hommel's method: 
1. The new p threshold (A. J. SANKOH, M. F. HUQUE AND S. D. DUBEY:  STATISTICS IN MEDICINE, VOL. 16, 2529-42 (1997)).
2. The adjusted p values (S.P. Wright: Biometrics 48:1005-13 (1992)).

This program does not need installation. In Linux, remember to set the execute permission of the program file.
 
Usage:
1. set the type I error (default: 0.05)
2. open a text file containing an array of p values (1 value per row, separated by CR/LF. Decimal separator must be ".").
3. the data appear in a grid ("p (original)") in decreasing order. Verify them if necessary. They cannot be modified in the program
4. adjusted p values appear in the adjacent grid ("p (adjusted)")
5. the p threshold corresponding to the type I error appears in the appropriate box
6. p threshold and old and new p values are saved in a file named appending "_p_adjusted" to the original file name

The text file containing the p values can be generated pasting a column from a spreadsheet into a text editor (e.g. notepad in Windows, kate/kwrite in Linux). Remove the row containing the field name, if present. Remember to paste data with a sufficient precision (at least 3 decimals). The list of p values should contain all the comparisons made, included those clearly not significant. 
