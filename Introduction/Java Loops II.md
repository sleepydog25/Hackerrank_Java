# Java Loops II
https://www.hackerrank.com/challenges/java-loops/problem

## Input / output
### Sample Input

2 
0 2 10 
5 3 5 
### Sample Output

2 6 14 30 62 126 254 510 1022 2046 
8 14 26 50 98 

## code
```java=
import java.util.*;
import java.io.*;

class Solution{
    public static void main(String []argh){
        Scanner in = new Scanner(System.in);
        int t=in.nextInt();
        while(in.hasNext()){
            int a = in.nextInt();
            int b = in.nextInt();
            int n = in.nextInt();
            math(a,b,n);
            System.out.println(" ");
        }
        in.close();
    }
    
    public static void math(int a, int b, int n){
        int ans = a;
        for (int i=0; i<n; i++){
            ans += (int)Math.pow(2,i)*b;
            System.out.print(ans + " ");
        }
    }
}

```
