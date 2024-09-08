# Java Primality Test
https://www.hackerrank.com/challenges/java-primality-test/problem

## Description
#### Sample Input

13
#### Sample Output

prime

## Code
```java
import java.io.*;
import java.math.*;
import java.security.*;
import java.text.*;
import java.util.*;
import java.util.concurrent.*;
import java.util.function.*;
import java.util.regex.*;
import java.util.stream.*;
import static java.util.stream.Collectors.joining;
import static java.util.stream.Collectors.toList;



public class Solution {
    public static void main(String[] args) throws IOException {
        BufferedReader bufferedReader = new BufferedReader(new InputStreamReader(System.in));

        String n = bufferedReader.readLine();
        BigInteger bigInt = new BigInteger(n);
        if (bigInt.isProbablePrime(1) == true)
          System.out.println("prime");
        else 
          System.out.println("not prime");

        bufferedReader.close();
    }
}

```
