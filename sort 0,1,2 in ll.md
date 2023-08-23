# sort 0,1,2 in ll
```
/*
class Node
{
    int data;
    Node next;
    Node(int data)
    {
        this.data = data;
        next = null;
    }
}
*/
class Solution
{
    //Function to sort a linked list of 0s, 1s and 2s.
    static Node segregate(Node head)
    {
        // add your code here
        int count[]={0,0,0};
        Node temp=head;
        while(temp!=null){
            count[temp.data]++;
            temp=temp.next;
        }
        temp=head;
        int i=0;
        while(i<3){
            if(count[i]==0){
                i++;
            }
            else{
                temp.data=i;
                count[i]--;
                temp=temp.next;
            }
        }
        
        return head;
        
    }
}


```
![image](https://github.com/sri-singhal/DSA-JAVA-/assets/98937798/3049b0d1-4b03-4adf-a0d1-af24859f309e)
