# EX 6D BRUTE FORCE ALGORITHM
## DATE:
## AIM:
To write a python program using brute force method of searching for the given substring in the main string.
## Algorithm
1. Take two inputs: the main string and the substring to search for.
2. Create a regex pattern using the substring.
3. Search for the first match of the pattern in the main string.
4. If a match is found.Print the starting index of the match.
5. Continue searching for the next match, starting just after the current match.
6. Repeat step 4 until no more matches are found.
## Program:
```
/*
To implement the program using brute force method of searching for the given substring in the main string.
Developed by: Subalakshmi V
Register Number:  212222040162
*/
```
```
import re
def match(string,sub):
    pattern = re.compile(str2)
    r = pattern.search(str1)
    while r:
        print("Found at index {}".format(r.start()))
        r = pattern.search(str1,r.start()+1)    

str1=input()
str2=input()
```
## Output:
![image](https://github.com/user-attachments/assets/aa14a3c7-cff3-402b-ae2b-929fb926acbf)

## Result:
Thus the above program was executed successfully for searching the substring at respective index.
