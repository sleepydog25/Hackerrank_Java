# Java Output Formatting
https://www.hackerrank.com/challenges/java-output-formatting/problem?isFullScreen=true

## outPut 
### Sample Input

java 100<br>
cpp 65<br>
python 50<br> 

### Sample Output

================================<br>
java           100 <br>
cpp            065 <br>
python         050 <br>
================================<br>

## Answer
```java
import java.util.Scanner;

public class Solution {

    public static void main(String[] args) {
            Scanner sc=new Scanner(System.in);
            System.out.println("================================");
            for(int i=0;i<3;i++)
            {
                String s1=sc.next();
                int x=sc.nextInt();
                System.out.printf("%-15s",s1);
                System.out.printf("%03d %n",x);
            }
            System.out.println("================================");

    }
}
```
