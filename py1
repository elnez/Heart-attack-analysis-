#This is a python test file

import string
fhand = open('file.txt')
counts = dict()
for line in fhand:
    line = line.translate(None, string.punctuation)
    line = line.lower()
    words = line.split()
    for word in words:
        if word not in counts:
            counts[word] = 1
        else:
            counts[word] += 1

# Sort the dictionary by value
lst = list()
for key,val in counts.items():
    lst.append((val,key))

lst.sort(reverse=True)

for key,val in lst[:1]:
    print key,val
