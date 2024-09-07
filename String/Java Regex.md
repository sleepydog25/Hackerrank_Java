# Java Regex
https://www.hackerrank.com/challenges/java-regex/problem

## Description
#### Sample Input

000.12.12.034
121.234.12.12
23.45.12.56
00.12.123.123123.123
122.23
Hello.IP
#### Sample Output

true
true
true
false
false
false

## Code
```java
import java.util.regex.Matcher;
import java.util.regex.Pattern;
import java.util.Scanner;

class Solution{

    public static void main(String[] args){
        Scanner in = new Scanner(System.in);
        while(in.hasNext()){
            String IP = in.next();
            System.out.println(IP.matches(new MyRegex().pattern));
        }

    }
}


//Write your code here
class MyRegex{
    String pattern = "^(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\."
                    + "(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\."
                    + "(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\."
                    + "(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)$";
}
```

## Notes
- ^: Asserts the start of the string.
- (225[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?): Matches numbers from 0 to 255.
- 25[0-5] matches 250-255.
- 2[0-4][0-9] matches 200-249.
- [01]?[0-9][0-9]? matches 0-199.
- \\.: Matches the dot .. (The dot is escaped because it is a special character in regex).
- $: Asserts the end of the string.
