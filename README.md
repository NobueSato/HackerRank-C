Problem

Objective 
This challenge will let you learn about bitwise operators in C.
Inside the CPU, mathematical operations like addition, subtraction, multiplication and division are done in bit-level. To perform bit-level operations in C programming, bitwise operators are used which are explained below. 
Bitwise AND operator & The output of bitwise AND is 1 if the corresponding bits of two operands is 1. If either bit of an operand is 0, the result of corresponding bit is evaluated to 0. It is denoted by &. Bitwise OR operator | The output of 
bitwise OR is 1 if at least one corresponding bit of two operands is 1. It is denoted by OR.
Bitwise XOR (exclusive OR) operator ^ The result of bitwise XOR operator is 1 if the corresponding bits of two operands are opposite. It is denoted by XOR

For example, for integers 3 and 5,

3 = 00000011 (In Binary)
5 = 00000101 (In Binary)

AND operation        OR operation        XOR operation
  00000011             00000011            00000011
& 00000101           | 00000101          ^ 00000101
  ________             ________            ________
  00000001  = 1        00000111  = 7       00000110  = 6


Task
Given set, s= {1,2,3,4......n} find:
the maximum value of a&b which is less than a given integer k , where a and b (where a < b) are two integers from set S. 
the maximum value of a|b which is less than a given integer k, where a and b (where a < b) are two integers from set S.
the maximum value of a XOR b which is less than a given integer k, where a and b (where a < b) are two integers from set S.

Input Format
The only line contains 2 space-separated integers n, and k, respectively.

Constraints
 2<=n<=10^3
 2<=k<=n

Output Format
The first line of output contains the maximum possible value of  a & b.
The second line of output contains the maximum possible value of  a | b.

 
The second line of output contains the maximum possible value of  a XOR b.

Sample Input :
5 4

Sample Output :
2
3
3

Explanation :
n = 5, k =4
S = {1,2,3,4,5}
All possible values of a and b are:
a = 1, b = 2 ; a&b = 0  a|b = 3  a XOR b = 3
a = 1, b = 3 ; a&b = 1  a|b = 3  a XOR b = 2
a = 1, b = 4 ; a&b = 0  a|b = 5  a XOR b = 5
a = 1, b = 5 ; a&b = 1  a|b = 5  a XOR b = 4
a = 2, b = 3 ; a&b = 2  a|b = 3  a XOR b = 1
a = 2, b = 4 ; a&b = 0  a|b = 6  a XOR b = 6
a = 2, b = 5 ; a&b = 0  a|b = 7  a XOR b = 7
a = 3, b = 4 ; a&b = 0  a|b = 7  a XOR b = 7
a = 3, b = 5 ; a&b = 1  a|b = 7  a XOR b = 6
a = 4, b = 5 ; a&b = 4  a|b = 5  a XOR b = 1 
The maximum possible value of a&b that is also <(k=4) is 2, so we print 2 on first line.
The maximum possible value of a|b that is also <(k=4) is 3, so we print 3 on first line.