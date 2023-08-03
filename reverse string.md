# Reverse String
```
class Reverse
{
    // Complete the function
    // str: input string
    public static String reverseWord(String str)
    {
        // Reverse the string str
        String rev="";
        int n= str.length();
        for(int i=n-1;i>-1;i--){
           rev=rev+str.charAt(i); 
        }
        return rev;
    }
}
```
![Screenshot (627)](https://github.com/sri-singhal/DSA-JAVA-/assets/98937798/ffa9b248-9a23-4375-95ef-ade01c7bafce)
