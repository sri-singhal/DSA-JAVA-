# print no. of duplicates in 2 strings at same index
```
class Solution 
{ 
    int sameChar(String A, String B) 
    {   A=A.toLowerCase();
        int count=0;
        B=B.toLowerCase();
        for(int i=0;i<A.length();i++){
            if(A.charAt(i)==B.charAt(i)){
                count++;
            }
        }
        return count;
        // code here
    }
}
```
![image](https://github.com/sri-singhal/DSA-JAVA-/assets/98937798/ad9e005a-094e-456a-8157-f0379d6e8fac)
