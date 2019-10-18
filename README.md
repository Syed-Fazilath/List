Code:
N = int(input())
A=[]
for i in range(N):
    x = list(map(str,input().split()))
    if "insert" in x:
        A.insert(int(x[1]),int(x[2]))
    elif "print" in x:
        print(A)
    elif "remove" in x:
        A.remove(int(x[1]))
    elif "append" in x:
        A.append(int(x[1]))
    elif "sort" in x:
        A.sort()
    elif "pop" in x:
        A.pop()
    elif "reverse" in x:
        A.reverse()
