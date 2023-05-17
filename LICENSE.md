public class FactorialCalculator {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Введите число: ");
        int number = scanner.nextInt();

        long factorialSum = 0;
        for (int i = 1; i <= number; i++) {
            factorialSum += factorial(i);
        }
