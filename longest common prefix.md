# longest common prefix
```
/*class Solution {
    public String longestCommonPrefix(String[] strs) {
        String pre="";
        int l=strs.length;
        if (l==1){
            return strs[0];
        }
        Arrays.sort(strs, Comparator.comparing(s->s.length()));
        int j=0;
        
    while(j<strs[0].length()){
        for(int i=1;i<l;i++){
              char k=strs[i].charAt(j);
              char c=strs[0].charAt(j);
              if(k!=c){
                  return pre;
              }
              

        }
        j++;
        pre+=strs[0].charAt(j - 1);
    }
     return pre;
 }
}


*/

//efficient Approach

class Solution {
    public String longestCommonPrefix(String[] strs) {
        int n = strs.length;
       
       String result = strs[0];
       
       
       for(int i = 1; i < n; i++){
            
            while(strs[i].indexOf(result) != 0){
               
               
                result = result.substring(0, result.length()-1);
               
                
                if(result.isEmpty()){
                    return "";
                }
            }
        }
        return result;

 }
}

```
![image](https://github.com/sri-singhal/DSA-JAVA-/assets/98937798/6ed8a542-7662-4e50-94bc-6abc429eda21)
   

 }
}
```
![image](https://github.com/sri-singhal/DSA-JAVA-/assets/98937798/6ed8a542-7662-4e50-94bc-6abc429eda21)
