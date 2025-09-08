# Ex. No: 15B - Build a Binary Search Tree Using Built-in Function

## AIM:
To write a Python program to build a binary search tree using a built-in function.

---

## ALGORITHM:

1. **Start the program.**
2. Define `_build_bst_from_sorted_values(sorted_values)` to recursively build a binary search tree (BST) from a sorted list.
3. Define `left_subtree(l)` to print the left subtree of the BST.
4. Take user input for the number of elements and store the values in a list `a`.
5. Sort the list and pass it to `_build_bst_from_sorted_values()` to construct the BST.
6. Print the postorder traversal of the BST.
7. Call `left_subtree(l)` to print the left subtree.
8. Check whether the tree is a binary search tree using the `is_bst` property.
9. **End the program.**

---

## PROGRAM:

```
Reg.No:212223060305
Name: Vishnu Priya E
from binarytree import Node
def _build_bst_from_sorted_values(sorted_values):
    if len(sorted_values) == 0:
        return None
    mid_index = len(sorted_values) // 2
    root = Node(sorted_values[mid_index])
    root.left = _build_bst_from_sorted_values(sorted_values[:mid_index])
    root.right = _build_bst_from_sorted_values(sorted_values[mid_index + 1 :])  
    return (root)

def left_subtree(l):
  print("Left Subtree : ")
  for i in l[1].values:
    print(i,"-->",end="")
  return 

a=[]
size=int(input())
for i in range(0,size):
  val=int(input())
  a.append(val)
x=sorted(a)


l=_build_bst_from_sorted_values(x)
print("Postorder :",l.postorder)
left_subtree(l)
print("\nIs this a Binary Search Tree? ",l.is_bst)

```

## OUTPUT

<img width="1769" height="540" alt="image" src="https://github.com/user-attachments/assets/d352de98-7d6b-4a4b-a8cb-6dd5c253a455" />

## RESULT
Thus, the Python program to build a binary search tree using a built-in function is implemented and executed successfully.
