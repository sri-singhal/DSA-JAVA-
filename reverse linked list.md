# reverse linked list
```
/**
 * Definition for singly-linked list.
 * public class ListNode {
 *     int val;
 *     ListNode next;
 *     ListNode() {}
 *     ListNode(int val) { this.val = val; }
 *     ListNode(int val, ListNode next) { this.val = val; this.next = next; }
 * }
 */
class Solution {
    public ListNode reverseList(ListNode head) {
        ListNode temp=head;
        ListNode prev=null;
        
       while(temp!=null){
           ListNode next=temp.next;
             temp.next=prev;
             prev =temp;
             temp=next;
       }
       return prev;
    }
}
```
![image](https://github.com/sri-singhal/DSA-JAVA-/assets/98937798/4d9b5107-28c3-4b4b-8ba9-33451b7f4621)
