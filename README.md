# Frequency-Difference
You're given a string s containing 'A' or 'B' only. Print the absolute difference the count of the frequencies of A and B. Input You're given a string s.  Constraints 1 &lt;= |s| &lt;= 105 Output Print the absolute difference between the frequencies. 

import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        
        String s = scanner.nextLine();

       
        int countA = 0;
        int countB = 0;

        for (char ch : s.toCharArray()) {
            if (ch == 'A') {
                countA++;
            } else if (ch == 'B') {
                countB++;
            }
        }

        int absoluteDifference = Math.abs(countA - countB);
        System.out.println(absoluteDifference);
    }
}
