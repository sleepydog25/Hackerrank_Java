# Java String Reverse
https://www.hackerrank.com/challenges/java-string-reverse/problem

## Description
palindrome

#### Sample Input

madam
#### Sample Output

Yes

## Code
```java
import java.io.*;
import java.util.*;

public class Solution {

    public static void main(String[] args) {
        
        Scanner sc=new Scanner(System.in);
        String A=sc.next();
        
        int left =0;
        int right = A.length()-1;
        
        while(left<right){
            if (A.charAt(left)!=A.charAt(right)){
              System.out.println("No");
              System.exit(0);
            }
            left++;
            right--;
        }
        System.out.println("Yes");
        
    }
}




```
