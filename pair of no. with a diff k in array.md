# pair of no. with diff k in array exists or not
```
class Solution
{
    public boolean findPair(int arr[], int size, int n)
    {
        //code here.
        Arrays.sort(arr);
        int maxdiff=arr[size-1]-arr[0];
        if (maxdiff<n){
            return false;}
        else{int k=0;
        for(int i=0;i<size;i++){
            for(int j=0;j<size;j++){
                if(i==j){
                    continue;
                }
                k=Math.abs(arr[j]-arr[i]);
                if (k==n ){
                return true;
                }
            }
        }
        return false;}
    }
}
```
![image](https://github.com/sri-singhal/DSA-JAVA-/assets/98937798/fc89768e-2db9-4933-92d5-80181a630745)
