# LogEntry
Reordering a Log Entry
Log Entry
You have been given a task of reordering some data from a log file. In the log file, every line is a space-delimited list of strings; a  lines begins with an alphanumeric identifier. There will be no lines consisting only of an identifier. 
After the alphanumeric identifier, a line will consist of either:
- a list of words using English letters, 
- or a list of only integers.

You have to reorder the data such that all of the lines with words are at the top of the log file. The lines with words are ordered lexicographically, ignoring the identifier except in the case of ties (if there are two lines that are identical except for the identifier), the identifier is used to order 
lexicographically. Alphanumeric should be sorted in ASCII order (numbers come before letters). The identifiers must still be part of the lines in the output Strings. Lines with integers must be left in the original order they were in the file. 
Write an algorithm to reorder the data in the log file, according to the rules above.

Input 
The input to the function/method consists of two arguments:
 - logFileSize, an integer representing the number of lines in the log file; 
 - logLines, a list of strings representing the log file

Output 
Return a list of strings representing the reordered log file data.

Note
Identifier consists of only english letters and numbers.
The lines with words are not required to match case and the sort needs to be case insensitive.

Example
Input:
logFileSize = 5
logLines = 
[a1 9 2 3 1]
[g1 Act cr]
[zo4 4 7]
[ab1 off KEY dog]
[a8 act zoo]

Output
[g1 Act car]
[a8 act zoo]
[ab1 off KEY dog]
[a1 9 2 3 1]
[zo4 4 7]

Explanation:
Second, fourth and fifth lines with words. According to the lexicographical order, the second 
line will be reordered first in the log file, then fifth, and the fourth comes in the log file. 
Next, the lines with numbers come in the order in which these lines were in the input.  
