### Sieve of Eratosthenes
- It is an algorithm for finding prime numbers from m  to  n 
- It consist of sieve or array of having m to n 
-  supppose a sieve of 1 to 5 so we start with 2 and mark all the multiples of 2 as false and than 
-  same procedure and find factorial of all those multiples which have mark as true to false 

## question 
- leetcode 204 
- GFG[Code here](https://practice.geeksforgeeks.org/problems/find-prime-numbers-in-a-range4718/1/)





## code
```java int count = 0;
        boolean[] prime = new boolean[n+1];
        for(int i = 0 ; i<n;i++)
        {
            prime[i] = true;
        }
        for(int i =2;i*i<n;i++)
        {
            if(prime[i]==true)
            {
                for(int j = i*i;j<=n;j=j+i)
                {
                    prime[j]=false;
                }
                
            }
       }`
       
   
       
       
   
