# web-data-extraction
# Came across Regular expression today in Py4E on coursera. First day. Thought it was interesting way to learn new things within python. Here is the program to extract specific data from .txt file :)
# extracts and sums up all the numbers within given data
import re

x = open('word.txt')
sum =0
y = re.findall('[0-9]+',x.read())
#print(y)
for i in y:
    num = int(i)
    sum += num
print(sum)
