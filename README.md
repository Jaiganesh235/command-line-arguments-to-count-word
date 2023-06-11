# command-line-arguments-to-count-word
## AIM:
To write a python program for getting the word count from the contents of a file using command line arguments.
## EQUIPEMENT'S REQUIRED: 
PC,Anaconda - Python 3.7
## ALGORITHM: 
### Step 1:
Import sys module to use command line arguments.
### Step 2: 
Use the open() by getting the file name with "sys.argv[1]" which means the first index of given argument. 
### Step 3: 
Iterate the content of the file using for loop.
### Step 4:  
Split the contents into each line using .split() function.
### Step 5: 
Iterate the list of lines and increment the value of variable (word) each time.
### Step 6: 
Run the program by giving "python prgm.py EX12.txt" on the terminal.

## PROGRAM:
```
#Developed By: S.Jaiganesh
#Register No: 212222240037
import sys
count = {}
with open(sys.argv[1], 'r') as f:
    for line in f:
        for word in line.split():
            if word not in count:
                count[word] = 1
            else:
                count[word] += 1
print(count)
f.close()
```
### File content:
![image](https://github.com/Jaiganesh235/command-line-arguments-to-count-word/assets/118657189/0eedc243-1703-439b-b594-320a7c582850)


## OUTPUT:
![image](https://github.com/Jaiganesh235/command-line-arguments-to-count-word/assets/118657189/59f9295d-a328-4c32-8206-f794124ff5e2)



## RESULT:
Thus the program is written to find the word count from the contents of a file using command line arguments.
