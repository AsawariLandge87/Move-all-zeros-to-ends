public class Main {
    public static void main(String[] args) {
        int[] arr = {0, 1, 0, 3, 12, 0};
        int arrNumber = 0;

  // Step 1: Move non-zero elements to front
        for (int i = 0; i < arr.length; i++) {
            if (arr[i] != 0) {
                arr[arrNumber] = arr[i];
                arrNumber++;
            }
        }

  // Step 2: Fill remaining with 0s
        while (arrNumber < arr.length) {
            arr[arrNumber] = 0;
            arrNumber++;
        }

        // Print result
        System.out.print("Result: ");
        for (int i = 0; i < arr.length; i++) {
            System.out.print(arr[i] + " ");
        }
    }
}
