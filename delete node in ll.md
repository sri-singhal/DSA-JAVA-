# delete node in ll
```
/*
class Node
{
	int data ;
	Node next;
	Node(int d)
	{
		data = d;
		next = null;
	}
}
*/

//Function to delete a node without any reference to head pointer.
class Solution
{
    void deleteNode(Node del)
    {
         // Your code here
         Node temp;
         temp=del;
         temp.data=del.next.data;
         temp.next=del.next.next;
         
         del=null;
         
         
    }
}
```
![image](https://github.com/sri-singhal/DSA-JAVA-/assets/98937798/6ed3a40c-5a34-4fbe-a544-56a480586de0)
