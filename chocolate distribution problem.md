# chocolate distribution problem 
```
// n length array and m students
//each element of array is a packet \
//each student should get 1 packet
class Solution
{
    public long findMinDiff (ArrayList<Integer> a, int n, int m)
    {   if(m<n+1){
        Collections.sort(a);
        long min=Integer.MAX_VALUE;
        for(int i=0;i<n-m+1;i++){
            
                if(a.get(m+i-1)-a.get(i)<min){
                    min =a.get(m+i-1)-a.get(i);
                }
                    
                
            }
            return min;
        }
        else{
            return -1;
        }
        
        // your code here
    }
}
```
![image](https://github.com/sri-singhal/DSA-JAVA-/assets/98937798/4ff6f8fe-422b-4339-a040-c126ea3268e9)
