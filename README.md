#fib on tree recursions 0 1 1 2 3 5 8 

def fib(n):
    if n<=1:
        return n
    return fib(n-1)+fib(n-2)
terms=int(input("enter number of terms to print:"))
print(("fibonacci series......"))
for i in range(terms):
    print(fib(i),end=' ')
''''''''''output''''''''''''''
enter number of terms to print: 6
fibonacci series......
0 1 1 2 3 5 



'''permutations of char in tree recursion'''
def permute(s, bucket=''):
    if not s:
        print(bucket)
        return
    for i in range(len(s)):
        ns=s[:i]+s[i+1:]
        permute(ns,bucket+s[i])
text=input("enter a name/word:")
print("possibilities of combinations....")
permute(text)
''''''''''output''''''''''''''
enter a name/word: abc
possibilities of combinations....
abc
acb
bac
bca
cab
cba


#length of binary string
def binary(n,b=' '):
    if n==0:
        print(b)
        return
    binary(n-1,b+'0')
    binary(n-1,b+'1')
length=int(input("enter length of string:"))
print("binary combinations.....")
binary(length)
''''''''''output''''''''''''''
enter length of string: 3
binary combinations.....
 000
 001
 010
 011
 100
 101
 110
 111



 #length of binary string
def binary(n,b=' '):
    if n==0:
        print(b)
        return
    binary(n-1,b+'0')
    binary(n-1,b+'1')
length=int(input("enter length of string:"))
print("binary combinations.....")
binary(length)
''''''''''output''''''''''''''
enter length of string: 4
binary combinations.....
 0000
 0001
 0010
 0011
 0100
 0101
 0110
 0111
 1000
 1001
 1010
 1011
 1100
 1101
 1110
 1111
