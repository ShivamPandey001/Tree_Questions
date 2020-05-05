#include <bits/stdc++.h> 
using namespace std; 
  
// A Binary Tree Node 
struct Node 
{ 
    int data; 
    struct Node *left, *right; 
}; 
  
void printLevelOrder(Node *root) 
{ 
    
    if (root == NULL)  return; // Base Case 
    queue<Node *> q; // Create an empty queue for level order tarversal 
    q.push(root); // Enqueue Root and initialize height
  
    while (q.empty() == false) 
    { 
        // Print front of queue and remove it from queue 
        Node *node = q.front(); 
        cout << node->data << " "; 
        q.pop(); 
  
        /* Enqueue left child */
        if (node->left != NULL) 
            q.push(node->left); 
  
        /*Enqueue right child */
        if (node->right != NULL) 
            q.push(node->right); 
    } 
} 
   
Node* newNode(int data) 
{ 
    Node *temp = new Node; 
    temp->data = data; 
    temp->left = temp->right = NULL; 
    return temp; 
} 
  
// Driver program
int main() 
{ 
    // Let us create binary tree shown in above diagram 
    Node *root = newNode(1); 
    root->left = newNode(2); 
    root->right = newNode(3); 
    root->left->left = newNode(4); 
    root->left->right = newNode(5); 
  
    cout << "Level Order traversal of binary tree is \n"; 
    printLevelOrder(root); 
    return 0; 
}
