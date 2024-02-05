# To execute:
1) mvn clean package
2) cd \target
3) java -jar .\licences-jar-with-dependencies.jar n (ej. 1000000)

# The License Plate Problem 
You work for the DMV; you have a specific, sequential way of generating new license plate numbers:
Each license plate number has 6 alphanumeric characters. The numbers always come before the letters.
The first plate number is 000000, followed by 000001. Finally, when you arrive at 999999, the next entry would be 00000A, Followed by 00001A. When you arrive at 99999A, the next entry is 00000B. After following the pattern to 99999Z, the next in the sequence would be 0000AA.
When 9999AA is reached, the next in the series would be 0000AB...
The pattern overview looks a bit like the following:
 
000000
000001
...
999999
00000A
00001A
...
99999A
00000B
00001B
...
99999Z
0000AA
0001AA
...
9999AA
0000AB
0001AB
...
9999ZZ
000AAA
001AAA
...
ZZZZZZ 
The goal is to write a function that takes some index n as a parameter and returns the nth element in this license plate sequence.
