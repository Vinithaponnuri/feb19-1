def myprime(n):
    x=n//2
    for i in range(2,x+1):
        if n%i==0:
            return False
    return True
t=int(input())
for i in range(t):
    x=input().split(' ')
    a=int(x[0])
    b=int(x[1])
    c=0
    for i in range(a+1,b):
        if myprime(i):
            c=c+1
    print(c)
