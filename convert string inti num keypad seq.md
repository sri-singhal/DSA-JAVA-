# convert string into num kypad seq
```
class Solution 
{ 
    String printSequence(String S) 
    { String arr[]={"2","22","222","3","33","333","4","44","444","5","55","555","6","66","666","7","77","777","7777","8","88","888","9","99","999","9999"};
      int len=S.length();
      String output="";
      for(int i=0;i<len;i++){
          if (S.charAt(i)==' '){
              output+="0";
          }
          else{
              int k= S.charAt(i)- 'A';
             output+=arr[k];
      }
      
      }
      return output;
        // code here
    }
}
```
![image](https://github.com/sri-singhal/DSA-JAVA-/assets/98937798/b7c70981-a115-4c41-a9fa-0beb0bc96f28)
