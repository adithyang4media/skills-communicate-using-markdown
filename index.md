# Welcome To My Github World
![Image of Yaktocat](https://octodex.github.com/images/yaktocat.png)
### Java program for number guessing game
```
import java.util.Scanner;

public class GuessMyNumber {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        int randomNumber = (int) (Math.random() * 100);

        System.out.println("I'm thinking of a number between 1 and 100. Try to guess it!");

        while (true) {
            int guess = scanner.nextInt();

            if (guess == randomNumber) {
                System.out.println("Correct! You guessed my number!");
                break;
            } else if (guess < randomNumber) {
                System.out.println("Your guess is too low.");
            } else {
                System.out.println("Your guess is too high.");
            }
        }

        scanner.close();
    }
}
```
