# Java Substring
https://www.hackerrank.com/challenges/java-substring/problem?isFullScreen=true

## Description
#### Sample Input

Helloworld  
3 7  

#### Sample Output

lowo

## Code 
```java
import java.io.*;
import java.util.*;
import java.text.*;
import java.math.*;
import java.util.regex.*;

public class Solution {

    public static void main(String[] args) {
        Scanner in = new Scanner(System.in);
        String S = in.next();
        int start = in.nextInt();
        int end = in.nextInt();
        
        //my code starts here
        String newWord = S.substring(start,end);
        System.out.print(newWord);
    }
}
```
