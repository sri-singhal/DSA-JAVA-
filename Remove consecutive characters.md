# Remove consecutive characters
```
class Solution{
    public String removeConsecutiveCharacter(String S){
        /*int k=S.length();
        int i=1;
        while(i<k){
            if (S.charAt(i)==S.charAt(i-1)){
                S=S.substring(0,i)+S.substring(i+1);
                k--;
            }
            else{
                i++;
            }
        }
        return S;*/
          
          
          //approach2 sliding window
          
          int j=0;
          int i=0;
          String news="";
          while(j<S.length()){
              
              if (S.charAt(j)==S.charAt(i)){
                  j++;
              }
              else if (S.charAt(j)!=S.charAt(i) || j==S.length()-1){
                  news+=S.charAt(i);
                  i=j;
                  j++;
              }
              
          }
          news+=S.charAt(j-1);
          return news;
          
    }
}
```
![image](https://github.com/sri-singhal/DSA-JAVA-/assets/98937798/fbb9b074-5108-46a8-b4ab-9ac042bc3d99)
