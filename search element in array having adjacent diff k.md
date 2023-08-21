# search element in array having adjacent diff k
```
class Complete{
    
   
    // Function for finding maximum and value pair
    public static int search (int arr[], int n, int x, int k) {
        //Complete the function
        
        // check existance of a no.
        int i=0;
        while(i<n){
             if(arr[i]==x){
                 return i;
             }
             i=i+Math.max(1,Math.abs((arr[i]-x)/k));
}
return -1;
    }
    
    
}




```
![image](https://github.com/sri-singhal/DSA-JAVA-/assets/98937798/57dc889d-cd1d-4999-9d1f-909521802d3c)
