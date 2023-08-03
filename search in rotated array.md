# Search in Rotated array
```
class Solution {
    public int search(int[] nums, int target) {
        for (int i=0;i<nums.length;i++){
            if(nums[i]==target){
                return i;
            }
        }
        return -1;
    }
}
```
![Screenshot 2023-08-04 010201](https://github.com/sri-singhal/DSA-JAVA-/assets/98937798/5ddde4ba-e984-4fa2-91b0-dc387f668c69)
