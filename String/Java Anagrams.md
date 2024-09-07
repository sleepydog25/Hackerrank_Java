# Java Anagrams
https://www.hackerrank.com/challenges/java-anagrams/problem

## Description
#### Sample Input 0

anagram
margana
#### Sample Output 0

Anagrams

## Code
```java
import java.util.Scanner;

public class Solution {

    static boolean isAnagram(String a, String b) {
        // my code starts here
        if (a.length()!= b.length())
          return false;
        
        int [] storage = new int [26];
        a = a.toLowerCase();
        b = b.toLowerCase();
        
        for (int i = 0; i < a.length(); i++) {
            storage[a.charAt(i) - 'a']++;
            }
            
        for (int k =0; k<b.length();k++){
            storage[b.charAt(k) - 'a']--;
        }
        
        for (int count:storage){
            if (count!= 0)
              return false;
        }
        
        return true; 
        // my code ends here
    }

  public static void main(String[] args) {
    
        Scanner scan = new Scanner(System.in);
        String a = scan.next();
        String b = scan.next();
        scan.close();
        boolean ret = isAnagram(a, b);
        System.out.println( (ret) ? "Anagrams" : "Not Anagrams" );
    }
}

```
