# Java End-of-file
## input
### Sample Input

>Hello world<br>
>I am a file<br>
>Read me until end-of-file.
### Sample Output

>1 Hello world<br>
>2 I am a file<br>
>3 Read me until end-of-file.<br>
## Answer
```java
import java.io.*;
import java.util.*;

public class Solution {

    public static void main(String[] args) {
        
        Scanner s = new Scanner(System.in);
        int count =1;
        while (s.hasNext()){
            String word = s.nextLine();
            System.out.println(count + " "+word);
            count++;
        }
        
    }
}

```
