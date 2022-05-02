## BIT POINTS 
- if a>>1 than it is divided by 2 
- if a<<1 than it is multiplied by 2 
- if you & any number with 1 than  if output is 1 than it is 1 and if output is 0 than it is even 
- SWAPPING 
-``` a = a^b
     b = a^b
     a = a^b
     ```
 - if you xor a to a than ouput is 0 and of a xor with 0 than its output is a 


 ### Questions
 - (56 Add Binary digits Leetcode ) 
 ``` 
 class Solution {
    public String addBinary(String a, String b) {
         StringBuilder sb = new StringBuilder();
       int i = a.length()-1;
        int j= b.length()-1;
        int carry = 0;
        int sum = 0;
        while(i>=0 || j>=0)
        {
            sum = carry;
            if(i>=0)
            {
            sum = sum + a.charAt(i)-'0';
            }
            if(j>=0)
            {
            sum = sum + b.charAt(j)-'0';
            }
            sb.append(sum%2);
            carry = sum/2;
         i--;
            j--;
            
            
        }
        if(carry!=0)
        {
            sb.append(carry);
        }
        return sb.reverse().toString();
        
        
        
        
    }
}
'''
