# Diameter-of-Binary-Tree
Explanation --
Diameter definition: The diameter of a binary tree is the number of nodes on the longest path between any two leaf nodes.
Objective -finds the longest path (diameter) in a binary tree.

Define Helper Function:

Create a function named help that takes a node as input.
Base Case:

In the helper function, check if the current node is null (empty). If it is, return 0.
Recursive Calls:

Recursively call the help function on the left and right child nodes of the current node.
Update Diameter:

Update the global variable diameter with the maximum value between itself and the sum of the heights of the left and right subtrees. diameter = max(diameter, left + right);
Return Height:

Return the maximum height of the left and right subtrees plus 1 (to account for the current node). return max(left, right) + 1;
Main Function:

Call the help function with the root node of the binary tree.
Initialize the diameter variable to 0.
Return Diameter:

After calling the helper function, return the value stored in the diameter.
Complexity:

Time complexity: O(n) visiting each node once.
Space complexity: O(h) due to recursive calls, where h is the tree's height.
