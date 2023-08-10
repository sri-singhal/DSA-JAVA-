# valid anagram

```
class Solution {
    public boolean isAnagram(String s, String t) {
        int len1=s.length();
        int len2= t.length();
        if(len1!=len2){
            return false;

        }
        int car=256;
        int count[]=new int[256];
        for(int i=0;i<len1;i++){
            count[s.charAt(i)]++;
            count[t.charAt(i)]--;
        }
        for(int i=0;i<car;i++){
            if(count[i]!=0){
                return false;
            }
        }
        return true;
    }
}
```
![image](https://github.com/sri-singhal/DSA-JAVA-/assets/98937798/941ca759-0a0e-4533-aeb3-8cef052c7156)
