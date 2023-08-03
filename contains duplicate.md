# Contains duplicate in array
```
class Solution {
    public boolean containsDuplicate(int[] nums) {
       /* Arrays.sort(nums);
        int a=nums[0];
        for(int i=1;i<nums.length;i++){
            if (nums[i]!=a){
                a=nums[i];
            }
            else{return true;}
        }
        return false;
*/

//better approach
 if(nums==null || nums.length==0)
            return false;
        HashSet<Integer> set = new HashSet<Integer>();
        for(int i: nums)
        {
            if(!set.add(i))
            {
                return true;
            }
        }
        return false;
        
    }
}
```
![image](https://github.com/sri-singhal/DSA-JAVA-/assets/98937798/11b684f3-faae-4ca3-ba96-064900eaea6c)
