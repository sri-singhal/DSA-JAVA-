# permutate two arrays such that corresponding sum>=k.md 
```
class Solution {
    public boolean isPossible(long a[], long b[], int n, long k) {
        Arrays.sort(a);
        Arrays.sort(b);
       for(int i=0;i<n;i++){
           if (a[i]+b[n-i-1]<k){
               return false;
           }
       }
       return true;
        // Your code goes here
    }
}
```
![image](https://github.com/sri-singhal/DSA-JAVA-/assets/98937798/00ce4149-5ca2-4341-a61e-aaab272a3f4e)
