# Number-Guessing-game-java-code
import java.util.*;
class Guess {

	public static void main(String[]args) {
		Scanner in = new Scanner(System.in);
		System.out.println("Guess the correct number ranging from 1 to 10.");
				while(true) {
			System.out.print("\nEnter a number ranging for 1 to 10: ");
			int n= in.nextInt();
    int r=(int)(Math.random() * 10) + 1;
			if (n < 1 || n > 10) {
			System.out.print("\nInvalid input! Enter a number ranging from 1 to 10.");
			} else if (n != r) {
				System.out.println("\nYou have guessed the wrong number! ");
				System.out.println("Your Number: " + n + " | Actual number: " + r);
			} else if (n == r) {
		System.out.println("\nYou have guessed the correct number! ");
				System.out.println("Your Number: " + n + " | Actual number: " + r);
				break;
	   }
	  }
  }
}
