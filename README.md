# FactorialCalculator
FactorialCalculator
import java.util.Scanner;

public class FactorialCalculator {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Введите число: ");
        int number = scanner.nextInt();

        long factorialSum = 0;
        for (int i = 1; i <= number; i++) {
            factorialSum += factorial(i);
        }

        System.out.println("Сумма факториалов чисел от 1 до " + number + ": " + factorialSum);
    }

    public static long factorial(int number) {
        long result = 1;
        for (int i = 2; i <= number; i++) {
            result *= i;
        }
        return result;
    }
}
