# Ex. No: 15C - Expression Tree with Inorder and Postorder Traversal

## AIM:
To write a Python program to build the given expression tree and print the inorder and postorder traversals.

---

## ALGORITHM:

1. **Start the program.**
2. Import the required modules (`build` and `Node` from `binarytree`).
3. Define a list `x` representing the expression tree in pre-order fashion (with `None` for missing nodes).
4. Use the `build()` function to generate the binary tree.
5. Print the **inorder** and **postorder** traversal of the tree.
6. **End the program.**

---

## PROGRAM:

```
name: Vishnu priya E
reg.no:212223060305

from binarytree import build,Node
x=['*',4,'-',5,'+',2,7]
t=build(x)
print(t.inorder)
print(t.postorder)
```

## OUTPUT
<img width="861" height="111" alt="image" src="https://github.com/user-attachments/assets/1fa118ee-a81c-40a9-b507-2882548da900" />


## RESULT
Thus the Python program to build the given expression tree and print the inorder and postorder traversals has been implemented and executed successfully.
