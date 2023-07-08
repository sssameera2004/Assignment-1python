Question 8:-

import math
import os
import random
import re
import sys



if __name__ == '__main__':
    n = int(input().strip())
    
    if n%2 != 0:
        print("Weird")
    elif n%2 == 0 and n>2 and n<=5:
        print("Not Weird")
    elif n%2 ==0 and n > 6 and n <=20:
        print("Weird")
    else:
        print("Not Weird")
 

Question 9:-
if __name__ == '__main__':
    alist = []
    for i in range(int(input())):
        name = input()
        score = float(input())
        alist.append([name, score])
second_highest = sorted(set([score for name, score in alist]))[1]
print('\n'.join(sorted([name for name, score in alist if score == second_highest])))


Question 10:-

if __name__ == '__main__':
    n = int(input())
    for i in range(n):
        print(i*i)

Question 11:-
def is_leap(year):
    leap = False
    
    # Write your logic here
    if year%4 == 0:            #Here we are checking if the year is normal year
        leap = True
        if year%100 == 0:        #Here we are checking if the year is a century year      
            if year%400 == 0:
                leap = True
            else:
                leap = False
        
                
    

                
    

    return leap

year = int(input())
print(is_leap(year))


Question 12:-

def count_substring(string, sub_string):
    total = 0
    for i in range(len(string)):
        if string[i:len(string)].startswith(sub_string):
            total += 1
    return total

if __name__ == '__main__':
    string = input().strip()
    sub_string = input().strip()
    
    count = count_substring(string, sub_string)
    print(count)


Question 13:-

if __name__ == '__main__':

    N = int(input())

    List=[];

    for i in range(N):

        command=input().split();

        if command[0] == "insert":

            List.insert(int(command[1]),int(command[2]))

        elif command[0] == "append":

            List.append(int(command[1]))

        elif command[0] == "pop":

            List.pop();

        elif command[0] == "print":

            print(List)

        elif command[0] == "remove":

            List.remove(int(command[1]))

        elif command[0] == "sort":

            List.sort();

        else:

            List.reverse();
