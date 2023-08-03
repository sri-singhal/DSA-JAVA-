# max subarray
```
class Solution {
    public int maxSubArray(int[] nums) {
        int maxsum=Integer.MIN_VALUE;
        int currentsum=0;
        for(int i=0;i<nums.length;i++){
             currentsum+= nums[i];
             if(currentsum>maxsum){
                 maxsum=currentsum;

             }
             if(currentsum<0){
                 currentsum=0;

             }
             
        }
        return maxsum;
    }
}
'''
![image](https://github.com/sri-singhal/DSA-JAVA-/assets/98937798/cded38e2-2b48-4ba3-bb65-25c0a831636c)
