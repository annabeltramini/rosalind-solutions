# rosalind-solutions
This repository contains all the Rosalind programming exercises I have solved,as well as the first solution I have found and new techniques I learned from it

### 1. Counting DNA Nucleotides
**My solution**
``` python
s= input()
A = 0
C = 0
G = 0
T = 0

for i in range (0,len(s)):
    if s[i] == "A":
        A += 1
    elif s[i] == "C":
        C += 1
    elif s[i] == "G":
        G += 1
    elif s[i] == "T":
        T += 1
print(A,C,G,T)
```
**Alternatives**
``` python
#1. Using .count() - fastest
s = input()
print(s.count("A"), s.count("G"), s.count("C"), s.count("T"))

#2 Using map() and unpacking the list - just one line of code
print(*map(input().count, "ACGT"))

#3 Using a dictionary - only loops once
s = input()
freq = {'A': 0, 'C': 0, 'G': 0, 'T': 0}
for i in s:
    freq[i] = freq[i] + 1
print(freq['A'], freq['C'], freq['G'], freq['T'])
```


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
