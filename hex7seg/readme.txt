Hex 7-segment display
Produces a 7-segment BugBoard display which displays hex numbers 0x0 through 0xF
Includes blaning in/out and decimal point drive.
Instructions:
Connect binary nybble (1 to 4 bits) to the "a" - "d" inputs ("a" = lsb). Unconnected state of all inputs = logic "0".
If blanking or DP not used, leave unconnected.
To use blanking, connect most-significant digit BO to next lowest digit BI.  Repeat for all digits except least
significant (leave its BI open).  DP will illuminate the decimal point and disable the BI/BO connections for that digit.
This allows dynamic decimal point selection with correct blanking behavior.  Here, "correct" means that the digit
to the left of the DP does not blank, nor do any digits to the right of the DP.
