# Valid Palindrome
```
import java.util.regex.Matcher;
import java.util.regex.Pattern;

class Solution {
    public boolean isPalindrome(String s) {
        String regex="[^A-Za-z0-9]";
        Pattern pattern= Pattern.compile(regex);
        Matcher matcher=pattern.matcher(s);
        String k= matcher.replaceAll("");
        String g=k.toLowerCase();
        int len=g.length();

        /*if (len%2==0){
            for (int i=0;i<len/2;i++){
                if(g.charAt(i)!=(g.charAt(len-1-i))){
                    return false;
                
                }
            }
            return true;

        }
        else{
            for (int i=0;i<len-1/2;i++){
                 if(g.charAt(i)!=(g.charAt(len-1-i))){
                    return false;
                
                }
            }
            
            return true;
            
        }*/




       // Approach 2
        int i=0;
        int j=len-1;
        while (i<j){
           if (g.charAt(i)!=g.charAt(j)){
               return false;
           }
           else{
               i++;
               j--;
           }
        }
        return true;
    }
}
```
![image](https://github.com/sri-singhal/DSA-JAVA-/assets/98937798/4c7a3b06-4bf2-48f0-ae92-45b675191cd7)
