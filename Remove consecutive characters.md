# Remove consecutive characters
```
class Solution{
    public String removeConsecutiveCharacter(String S){
        int k=S.length();
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
        return S;
    }
}
```
![image](https://github.com/sri-singhal/DSA-JAVA-/assets/98937798/fbb9b074-5108-46a8-b4ab-9ac042bc3d99)
