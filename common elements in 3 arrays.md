# common elements in 3 sorted arrays
```
   class Solution
{
    ArrayList<Integer> commonElements(int A[], int B[], int C[], int n1, int n2, int n3) 
    {
        // code here 
        int i=0;int j=0;
         ArrayList<Integer> temp=new ArrayList<>();
        int k=0;
        while(i<n1 && j<n2&& k<n3){
            if(A[i]==B[j] && B[j]==C[k]){
                
                temp.add(A[i]);
                i++;
                j++;
                k++;
                
            }
            
            
            
           else  if(A[i]<B[j]){
                 i++;
             }
             else if(B[j]<C[k]){
                 j++;
             }
             else{
                 
                 k++;
             }
        }
       int prevElement = Integer.MIN_VALUE;
        ArrayList<Integer> result = new ArrayList<>();
        for (int value : temp) {
            if (value != prevElement) {
                result.add(value);
                prevElement = value;
            }
        }

        return result;
        
    }
    
}
```
![image](https://github.com/sri-singhal/DSA-JAVA-/assets/98937798/d12cf069-1ed6-4ca6-b9b7-b67b5533c182)
        
