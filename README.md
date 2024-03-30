import java.util.Scanner;

public class NumberNames {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.println("Enter the number:");
        String number = scanner.nextLine().trim();
        scanner.close();

        String[] numberNames = {"zero", "one", "two", "three", "four", "five", "six", "seven", "eight", "nine"};

        // Iterate through each digit of the number and print its name
        for (int i = 0; i < number.length(); i++) {
            char digit = number.charAt(i);
            int index = Character.getNumericValue(digit);
            System.out.print(numberNames[index] + " ");
        }
    }
}
