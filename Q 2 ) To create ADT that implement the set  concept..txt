l1 = [0,0,0,0,0,0,0,0,0,0]
l2 = [0,0,0,0,0,0,0,0,0,0]

print(l1)
print(l2)

ch = 1
while(ch==1):
    key = int(input("Enter Key : "))
    d = key % 10
    for i in l1:
        if l1[d] > 0:
            d+=1
    l1[d]=key

    key = int(input("Enter Key : "))
    d = key % 10
    for i in l2:
        if l2[d] > 0:
            d +=1
    l2[d]=key

    print(l1)
    print(l2)
    ch = int(input("Enter Choice to continue or exit 0/1 : "))

# Delete operation 
while(ch==1):
    delete = int(input("Enter No to be Delete "))
    d = key % 10
    if l[d] > 0:
        l[d] = 0
    print(l1)
    ch = int(input("Enter Choice 0/1 : "))

# Traverse 
key = int(input("Enter key to search : "))
for i in range(10):
    if l1[i] == key:
        print("Searched : ",i)
    else:
        print("Not Available !")
        break


# Union
print("union")
l1=set(l1)
l2=set(l2)
u = l1.union(l2)
u = list(u)
print(u)

# Insertion 
print("Insertion")
i = l1.intersection(l2)
i = list(i)
print(i)

# Difference
print("Difference")
d = l1 - l2
d = list(d)
print(d)