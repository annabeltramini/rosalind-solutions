# rosalind-solutions
This repository contains all the Rosalind programming exercises I have solved,as well as the first solution I have found and new techniques I learned from it

### 1. Counting DNA Nucleotides



### 2. Transcribing DNA into RNA
**My solution**
``` python
s = input()
RNA = ""
for i in range(0,len(s)):
    if s[i] == "T":
    	RNA += "U"
    else:
        RNA += s[i]
        
print(RNA)
```
**Alternatives**
``` python
xxx
```
### 3. Complementing a strand of DNA
**My solution**
``` python
s = input()

s_3t5 = ""

bases = {"A":"T","G":"C","C":"G","T":"A"}
for i in range (0,len(s)):
    s_3t5 += bases[s[i]]
s_5t3 = s_3t5[::-1]
print(s_5t3)
    
```
**Alternatives**
``` python
xxx
```
