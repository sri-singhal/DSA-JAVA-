# counting sort
```

class Solution
{
    //Function to arrange all letters of a string in lexicographical 
    //order using Counting Sort.
    public static String countSort(String arr)
    {
        // code here
        int ar[]=new int[26];
        String k="";
        int l = arr.length();
        for(int i=0;i<l;i++){
            ar[Integer.valueOf(arr.charAt(i))-97]++;
        }
          for(int i=0;i<26;i++){
              for (int j=0;j<ar[i];j++){
                  k+=(char)(i+97);
              }
              
          }
          return k;
        
    }
}



```
![image](https://github.com/sri-singhal/DSA-JAVA-/assets/98937798/5d52ef82-5648-47d3-8ac4-7f3baf6f9f70)
