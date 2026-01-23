# ADDITIONAL EXPERIMENTS
# TITLE 1.) Inserting substring into main string
```
import java.util.Scanner;
public class InsertSubstring {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter the main string: ");
        String mainString = sc.nextLine();
        System.out.print("Enter the substring to insert: ");
        String subString = sc.nextLine();
        System.out.print("Enter the position to insert the substring: ");
        int position = sc.nextInt();
        if (position < 0 || position > mainString.length()) {
            System.out.println("Invalid position!");
        } else {
            String firstPart = mainString.substring(0, position);
            String secondPart = mainString.substring(position);
            String resultString = firstPart + subString + secondPart
            System.out.println("Resulting string: " + resultString);
        }
        sc.close();
    }
}
```

# OUTPUT 
![add1](https://github.com/user-attachments/assets/91e2001d-99b6-4fdd-8beb-54f3f194628e)

# TITLE 3.) Checking whether the string is palindrome or not 
```
import java.util.Scanner;
public class PalindromeCheck {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter a string: ");
        String str = sc.nextLine();
        int start = 0;
        int end = str.length() - 1;
        boolean isPalindrome = true;
        while (start < end) {
            if (str.charAt(start) != str.charAt(end)) {
                isPalindrome = false;
                break;
            }
            start++;
            end--;
        }
        if (isPalindrome) {
            System.out.println("String is a palindrome");
        } else {
            System.out.println("String is not a palindrome");
        }
        sc.close();
    }
}
```

# OUTPUT 
![add3](https://github.com/user-attachments/assets/5234bab8-ff46-4be5-ac44-603f453b28a9)

# TITLE 4.) Checking if a number is a perfect number
```
import java.util.Scanner;

public class PerfectNumber {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter a positive integer: ");
        int num = sc.nextInt();
        int sum = 0;
        for (int i = 1; i <= num - 1; i++) {
            if (num % i == 0) {
                sum = sum + i;
            }
        }
        if (sum == num) {
            System.out.println(num + " is a perfect number");
        } else {
            System.out.println(num + " is not a perfect number");
        }
        sc.close();
    }
}
```

# OUTPUT
![add4](https://github.com/user-attachments/assets/89c38da6-d407-4f46-8aa1-48bf6bb03a4b)




