# List
Consider a list (list = []). You can perform the following commands:  
insert i e: Insert integer e at position i. 
print: Print the list. 
remove e: Delete the first occurrence of integer e. 
append e: Insert integer e at the end of the list. 
sort: Sort the list. 
pop: Pop the last element from the list. 
reverse: Reverse the list. 
Sample Input:   10
                insert 0 5
                remove 5 
                append 9
                insert 1 4
                insert 2 3
                sort
                pop 
                reverse 
                print 
Sample Output:    [4,3]
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
