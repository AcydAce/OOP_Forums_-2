import java.util.Scanner;

class PrintArray {
    public static void main(String[] args) {

        int numItems;   //declaring variables
        int[] items;    //declaring array

        Scanner in = new Scanner(System.in);
        System.out.print("Enter The Number of Items (>-1): ");    // asks user input
        numItems = in.nextInt();

        items = new int[numItems];
        System.out.print("Enter value of all items (seperated by space): ");
        for (int i = 0; i < items.length; i++){
            items[i] = in.nextInt();
        }
        System.out.print("The values are: [");  // prints out the array
        for (int i = 0; i < items.length; i++) {
            System.out.print(items[i]);
            if (i != items.length-1) {          // adds "," in between the items
                System.out.print(", ");
            }
        }
        System.out.println("]");
    }
}
