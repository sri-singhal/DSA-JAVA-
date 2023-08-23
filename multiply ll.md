# multiply ll
```
/*Node is defined as
class Node
{
    int data; 
    Node next;
    Node(int data) {
        this.data=data;
        this.next = null;
    }
}*/

class GfG{
  /*You are required to complete this method */
   public long multiplyTwoLists(Node l1,Node l2){
          //add code here.
          long num=0;
          long num2=0;
          long n=1000000007;
          Node temp=l1;
          Node gemp=l2;
          while(temp!=null||gemp!=null){
              if(temp!=null){
                  num=(num*10)%n+temp.data;
                  temp=temp.next;
              }
              if(gemp!=null){
                  num2=(num2*10)%n+gemp.data;
                  gemp=gemp.next;
                  
              }
                  
          }
          long k=((num % n)*(num2 % n))% n;
          return k;
   }
}
```
![image](https://github.com/sri-singhal/DSA-JAVA-/assets/98937798/1ee38fd2-6a83-484b-9d46-84369d85225d)
