# check if ll has cycle or not
```
/**
 * Definition for singly-linked list.
 * class ListNode {
 *     int val;
 *     ListNode next;
 *     ListNode(int x) {
 *         val = x;
 *         next = null;
 *     }
 * }
 */
public class Solution {
    public boolean hasCycle(ListNode head) {
        ListNode s=head;
        ListNode f=head;

        while(f!=null && f.next !=null){
             s=s.next;
             f=f.next.next;
             if (s==f){
                 return true;
             }

        }
        
            return false;
        
    }
}
```
![image](https://github.com/sri-singhal/DSA-JAVA-/assets/98937798/41a5def8-95b8-4311-beb7-e98352a37249)


