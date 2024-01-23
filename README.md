AdventureGame {

public static void main(String[] args) {
    Scanner scanner = new Scanner(System.in);

    System.out.println("Welcome to the Text Adventure Game!");
    System.out.println("You find yourself in a mysterious forest. Choose your path wisely.");

    // Start of the game
    while (true) {
        System.out.println("\nOptions:");
        System.out.println("1. Go left into the dark cave.");
        System.out.println("2. Go right towards the enchanted waterfall.");
        System.out.println("3. Quit the game.");

        System.out.print("Enter your choice (1, 2, or 3): ");
        int choice = scanner.nextInt();

        switch (choice) {
            case 1:
                System.out.println("You enter the dark cave...");
                System.out.println("It's too dark to see anything. You get lost and the game ends.");
                break;
            case 2:
                System.out.println("You approach the enchanted waterfall...");
                System.out.println("Congratulations! You discover a hidden treasure behind the waterfall. You win!");
                break;
            case 3:
                System.out.println("Thanks for playing! Goodbye!");
                System.exit(0);
            default:
                System.out.println("Invalid choice. Please enter 1, 2, or 3.");
        }
    }
}
}
