# floor and ceil
```
class Solve {
    Pair getFloorAndCeil(int[] arr, int n, int x) {
        // code here
        int floor=-1;
        int ceil=-1;
        int k=Integer.MIN_VALUE;
        int g=Integer.MAX_VALUE;
        Arrays.sort(arr);
        if (arr[0]>x){
            ceil=arr[0];
        }
        else if(arr[n-1]<x){
            floor=arr[n-1];
        }
        else{
        for(int i=0;i<n;i++ ){
            if(arr[i]<=x&& arr[i]>k){
                k=arr[i];
                
            }
            if(arr[i]>=x && g>arr[i]){
                g=arr[i];
            }
            
        }
        floor=k;
        ceil=g;
        }

        return  new Pair(floor, ceil);
       
    }
}
```
![image](https://github.com/sri-singhal/DSA-JAVA-/assets/98937798/636f0e2e-2c2a-4e83-a22f-d2eb9a685906)

