# valid paranthesis
```
import java.util.HashMap;
import java.util.Stack;
class Solution {
    public boolean isValid(String s) {
      int len = s.length();
      HashMap<Character,Character> yo =new HashMap<>();
      yo.put('{','}');
      yo.put('(',')');
      yo.put('[',']');
      Stack<Character> stc= new Stack<>();
      int top =-1;
      int i=0;
      while( i<len){
          char k = s.charAt(i);
          if(yo.containsKey(k)){
              stc.push(k);
              i++;
              top++; 
          }
          else if(!stc.isEmpty() && (yo.get(stc.peek())==k)){
                stc.pop();
               top--;
               i++;
         }
          else{
              return false;
          }
          

      }
      if(top==-1){
          return true;
      }
       else
       {return false;}
    
    }
}
```
![image](https://github.com/sri-singhal/DSA-JAVA-/assets/98937798/940c084f-2a88-4c20-98e1-dd3b09817631)
