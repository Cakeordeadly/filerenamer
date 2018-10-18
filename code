import os       # for getting files from directory
import sys      # for accessing command line arguments
import csv

def readcsv(filename):	
    ifile = open(filename, "r")
    reader = csv.reader(ifile, delimiter=";")
    rownum = 0	
    a = []
    for row in reader:
        a.append (row)
        rownum += 1
    
    ifile.close()
    return a

folder_name = "C:/Users/Chris/Documents/Bin/"
with open("C:/Users/Chris/Documents/py/inlist.csv","r") as f:
    reader = csv.reader(f)
    in_list = list(reader)
i = len(in_list)
print(i)

for x in range(0,i):
    os.rename(folder_name + in_list[x][0], folder_name + in_list[x][1])
    print(folder_name + in_list[x][0])
