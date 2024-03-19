
package java_methods;
import java.util.Scanner;

public class methods {
   public static void main(String[] args) {
       
        findAndDisplayLargestAndSmallestNumbers();
    }

    public static void findAndDisplayLargestAndSmallestNumbers() {
        Scanner input = new Scanner(System.in);

        System.out.print("Enter three numbers: ");
        int num1 = input.nextInt();
        int num2 = input.nextInt();
        int num3 = input.nextInt();

        int largest, smallest;

        // Determine the largest and smallest numbers using if statements
        if (num1 >= num2 && num1 >= num3) {
            largest = num1;
        } else if (num2 >= num1 && num2 >= num3) {
            largest = num2;
        } else {
            largest = num3;
        }

        if (num1 <= num2 && num1 <= num3) {
            smallest = num1;
        } else if (num2 <= num1 && num2 <= num3) {
            smallest = num2;
        } else {
            smallest = num3;
        }

        // Display the results in the required format
        System.out.println("The smallest number: " + smallest);
        System.out.println("The largest number: " + largest);
        System.out.println(largest + " is your largest and " + smallest + " smallest number.");
    }
} 
