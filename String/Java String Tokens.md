# Java String Tokens
https://www.hackerrank.com/challenges/java-string-tokens/problem

## Description
#### Sample Input

He is a very very good boy, isn't he?
#### Sample Output

10   
He    
is<br>
a<br>
very<br>
very<br>
good<br>
boy<br>
isn<br>
t<br>
he<br>

## Code
```java
import java.io.*;
import java.util.*;

public class Solution {

    public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);
        String s = scan.nextLine();
        // my code starts here
        
        //spliting sentence
        
        String words [] = s.split("[^A-Za-z]+");
        int count = 0;
        for (String k: words){
            count++;
        }
        System.out.println(count);
        for (String k: words){
            System.out.println(k);
        }
        //my code ends here
        scan.close();
    }
}
```
