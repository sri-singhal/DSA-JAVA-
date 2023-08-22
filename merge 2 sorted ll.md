# merge 2 sorted ll
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
    public ListNode mergeTwoLists(ListNode start_1, ListNode start_2) {
       ListNode l3;
       if (start_1==null){
           return start_2;
       }
       else if(start_2==null){
           return start_1;
       }
       if(start_1.val< start_2.val){
           l3=start_1;
           start_1=start_1.next;
           
           

       }
       else{
           l3=start_2;
           start_2=start_2.next;

       }
       
       ListNode temp= l3;
       while(start_1!= null&& start_2!=null){
           if(start_1.val< start_2.val){
           temp.next=start_1;
           start_1=start_1.next;
           temp= temp.next;
           

       }
       else{
           temp.next=start_2;
           start_2=start_2.next;
             temp= temp.next;

       }
       }
       if (start_1==null){
          temp.next= start_2;
       }
       else if(start_2==null){
           temp.next= start_1;
       }
       
       return l3;
    }
}
    ```
![image](https://github.com/sri-singhal/DSA-JAVA-/assets/98937798/ea83bb17-3a8a-43c0-b9f0-e1a6c4ee2c43)
