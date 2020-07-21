# Same binary Tree: Given two binary trees, write a function to check if they are the same or not.
Two binary trees are considered the same if they are structurally identical and the nodes have the same value.
Example 1:
Input:

           1         1

          / \       / \

         2   3     2   3

        [1,2,3],   [1,2,3]

Output: true <br/>
Example 2: <br/>
Input:

           1         1

          /           \

         2             2

        [1,2],     [1,null,2]

Output: false <br/>
Example 3: <br/>
Input:

           1         1

          / \       / \

         2   1     1   2

        [1,2,1],   [1,1,2]

Output: false

```C++
// C++
#include <iostream>
using namespace std;
//  * Definition for a binary tree node.
struct TreeNode
{
    int val;
    TreeNode *left;
    TreeNode *right;
    TreeNode() : val(0), left(NULL), right(NULL) {}
    TreeNode(int x) : val(x), left(NULL), right(NULL) {}
    TreeNode(int x, TreeNode *left, TreeNode *right) : val(x), left(left), right(right) {}
};

bool isSameTree(TreeNode *p, TreeNode *q)
{
}
```