# massforscript


#https://github.com/Will-Dong/massforscript.git


import re
import os
a=open('..\do.txt')
b=open('F:\\result.txt','a')
reg=re.compile(r'Tap (\d){1,4},( )?(\d){1,4}')
while True:
    line = a.readline()
    if reg.search(line):
        b.write(line)
        print(line)
a.close()
b.close()
