# command-line-arguments-to-count-word
## AIM:
To write a python program for getting the word count from the contents of a file using command line arguments.
## EQUIPEMENT'S REQUIRED: 
PC
Anaconda - Python 3.7
## ALGORITHM: 
### Step 1:
Import the sys module.

### Step 2: 
Pass the filename as the first argument after the name of script.Open the file as sys.argv[1]
 
### Step 3: 
Read the file using read() method

### Step 4:  
Use split() method to split the file content into words.

### Step 5: 
Use len() to find the total words.

### Step 6: 
Run the program to determine the number of words in the file create


## PROGRAM:
```
Developed by: Aakashraj M
Register number: 22008579

import sys
fp=open(sys.argv[1],"r")
d={}
for i in fp:
    for w in i.split():
        if w not in d.keys():
            d[w]=1
        else:
            d[w]+=1
print(d)
```
### OUTPUT:
![image](https://user-images.githubusercontent.com/121117266/214827915-8c420297-1311-416f-a4fa-60f2598e76cf.png)
![image](https://user-images.githubusercontent.com/121117266/214827983-fa520275-22d5-46e3-967b-5c1673948796.png)

## RESULT:
Thus the program is written to find the word count from the contents of a file using command line arguments.
