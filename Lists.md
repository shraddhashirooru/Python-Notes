## i. Printing based on index:

```
my_list=["banana", "apple", "cherry", "lemon", "orange", "blueberry"]

item=my_list[1]
print(item) #print apple

item=my_list[-1]
print(item) #print last item that is blueberry

```

Output:

```
apple
blueberry
```

---
## ii. Slicing:

```
my_list=["banana", "apple", "cherry", "lemon", "orange", "blueberry"]

item=my_list[1:3]
print(item) #print first index and 2nd index those are apple and cherry

item=my_list[1:5:2]
print(item) #print apple to orange skip of 1

item=my_list[::-1]
print(item) #reverse the list
```

Output:

```
['apple', 'cherry']
['apple', 'lemon']
['blueberry', 'orange', 'lemon', 'cherry', 'apple', 'banana']
```

---
## iii. For loop to print the items one by one:

```
my_list=["banana", "apple", "cherry", "lemon", "orange", "blueberry"]

for i in my_list:
    print(i) # it print all items in my_list line by line
```

Output:

```
banana
apple
cherry
lemon
orange
blueberry
```

---
## iv. Check the item:

```
my_list=["banana", "apple", "cherry", "lemon", "orange", "blueberry"]

if "banana" in my_list:
    print("yes")
else:
    print("No") #check if particular item in the list
```

Output:

```
yes
```

---
## v. Print the length of list:

```
my_list=["banana", "apple", "cherry", "lemon", "orange", "blueberry"]

print(len(my_list)) #print the length of the list
```

Output:

```
6
```

---
## vi. Add item in the last:

```
my_list=["banana", "apple", "cherry", "lemon", "orange", "blueberry"]

my_list.append("jackfruit")
print(my_list)#add item to the last
```

Output:

```
['banana', 'apple', 'cherry', 'lemon', 'orange', 'blueberry', 'jackfruit']
```

---
## vii. Add item to the particular index:

```
my_list=["banana", "apple", "cherry", "lemon", "orange", "blueberry", “jackfruit”]

my_list.insert(3, "moosambi")
print(my_list)#add item to the 3 index
```

Output:

```
['banana', 'apple', 'cherry', 'moosambi', 'lemon', 'orange', 'blueberry', 'jackfruit']
```

---
## viii. Use of pop, remove and reverse:

```
my_list=["banana", "apple", "cherry", "lemon", "orange", "blueberry", “jackfruit”]

my_list.pop()#it remove last item
print(my_list)

my_list.remove("cherry") #to remove particular item
print(my_list)

my_list.reverse() #it reverse the list
print(my_list)
```

Output:

```
['banana', 'apple', 'cherry', 'moosambi', 'lemon', 'orange', 'blueberry']
['banana', 'apple', 'moosambi', 'lemon', 'orange', 'blueberry']
['blueberry', 'orange', 'lemon', 'moosambi', 'apple', 'banana']
```

---
## ix. Print the sorted list (increasing order): Both gives the same output:

```
My_list=['blueberry', 'orange', 'lemon', 'moosambi', 'apple', 'banana']

my_list.sort()

newlist=sorted(my_list)
```

Output:

```
['apple', 'banana', 'blueberry', 'lemon', 'moosambi', 'orange']
```

---
## x. +,* and copy in list:

```
list2=[1,3,56,8]*2 # it repeat add the same list again to it output: [1,3,56,8,1,3,56,8]
print(list2)

list3=[3,9,10]
list4=list2+list3 #to combine two list values
print(list4)

list5=list3.copy() #to copy the items from list 3 to list 5
print(list5)
```

Output:

```
[1, 3, 56, 8, 1, 3, 56, 8]
[1, 3, 56, 8, 1, 3, 56, 8, 3, 9, 10]
[3, 9, 10]
```

---
## xi. List compression and all() :

```
list3=[3,9,10]
mul=[i*i for i in list3] #all item in list3 squared and added to mul list.
print(mul)

a=[2,4,6,8]
ans=all(i%2==0 for i in a)
print(ans)
```

Output:

```
[9, 81, 100]
True
Second code check if all values are even, it return True only if all satisfy the condition.
```

---
### xii. Changing list value, counting and showing index of particular value:

```
mul=[9, 81,100]

mul[2]=45 #it change  the 3rd item to  45
print(mul)

print(mul.count(81)) #it count the number of 81 present in mul
print(mul.index(45)) #it shows the index of the number of 45 present in mul
```

Output:

```
[9, 81, 45]
1
2
```

---
## xiii. Unpacking and clearing list:

```
mul=[9, 81,100]

hermark, mymark, myfreindmark=mul #use for unpacking the elements in list
print(hermark)
my_list.clear() #it clear all item in the list
```

Output:

```
9
[]
```

----
## xiv. Unpacking or slicing:

```
newlist1=[2, 4, 6, 9, 8, 7]

i1, *i2, i3=newlist1
print(i2) #it print all element except first and last
print(i1) # it print first element
print(i3) #it print last element
```

Output:

```
[4, 6, 9, 8]
2
7
```

---
## xv. Extending the list with another list:

```
newlist1=[2, 4, 6, 9, 8, 7]

newlist2=[1, 4, 5]
newlist1.extend(newlist2)
print(newlist1)
```

---
Output:

```
[2, 4, 6, 9, 8, 7, 1, 4, 5]
```

---
## xvi. Access both index and value in the list using enumerate

```
for i, j in enumerate(b):
    print(f"{i}-{j}")
```

Output:

```
0-3
1-6
2-8
3-9
4-2
```
---
## xvii. Fining the particular number index in list

```
a=[10,15,20,45,10,20]

print(a.index(20))
print(a.index(20,(a.index(20)+1)))
```

Output:

```
2
5
First number index and second number index both can be find.
```

---
## xvii. Delete the specific value inside the list: (Knowing the index)

```
a=[1,2,3,4]
del a[0]
print(a)
```

Output:

```
[2, 3, 4]
```

---
## xviii. printing number from backwards

```
a=[2,3,8,9,10,11]

for i in range(len(a)-1,-1,-1):
    print(i)
```

Output:

```
5
4
3
2
1
0
```

It start from n-2 and stop before -1 and each iteration it jump -1 means decrease.
