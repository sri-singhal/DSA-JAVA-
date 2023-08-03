# sum of min max of an array
```class Solution
{ 
    public static int findSum(int A[],int N) 
    {
        // Arrays.sort(A)
        // int min=A[0];
        //int max=A[N-1];


        int min=A[0];
        int max=A[0];
        
        if (N==1){
            return 2*A[0];
            
        }
        else{
            for(int i=1;i<N;i++){
               if(A[i]<min){
                   min=A[i];
               }
               if (A[i]>max){
                   max=A[i];
               }
            }
        }
        int sum=max+min;
        return sum;
       
    }
}
```
![Screenshot (625)](https://github.com/sri-singhal/DSA-JAVA-/assets/98937798/4b650ec8-2e3f-4ee3-abd9-46b42c8292b4)


