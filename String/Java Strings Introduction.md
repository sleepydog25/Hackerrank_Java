# Java Strings Introduction
https://www.hackerrank.com/challenges/java-strings-introduction/problem?isFullScreen=true
## Description
There are three lines of output:
For the first line, sum the lengths of  and .
For the second line, write Yes if  is lexicographically greater than  otherwise print No instead.
For the third line, capitalize the first letter in both  and  and print them on a single line, separated by a space.

#### Sample Input 0

hello  
java   
#### Sample Output 0

9  
No    
Hello Java  
## Code
```java
import java.io.*;
import java.util.*;

public class Solution {

    public static void main(String[] args) {
        
        Scanner sc=new Scanner(System.in);
        String A=sc.next();
        String B=sc.next();

        //my code starts here
        //Line one
        int total = A.length()+B.length();
        System.out.println(total);
        
        //Line two
        if(A.compareTo(B)>0)
          System.out.println("Yes");
        else
          System.out.println("No");
        
        //Line three
        String outputA = A.substring(0,1).toUpperCase() + A.substring(1);
        String outputB = B.substring(0,1).toUpperCase()+B.substring(1);
        System.out.println(outputA + " "+outputB);
        
    }
}
```
