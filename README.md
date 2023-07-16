# Problem-1.T2021-2-1

import java.util.Scanner;

public class SmallCalculator {
	public static void main(String[] args) {
		Scanner scan = new Scanner(System.in);
		SmallCalculator calculator = new SmallCalculator();

		System.out.println("Enter the value of 'a': ");
		double a = scan.nextDouble();

		System.out.println("Enter the value of 'b': ");
		double b = scan.nextDouble();

		System.out.println("Enter the type of operation +, -, *, / ");
		String operation = scan.next();

		double result;

		switch (operation) {
		case "+":
			result = calculator.add(a, b);
			System.out.println("Result: " + result);
			break;
		case "-":
			result = calculator.subtract(a, b);
			System.out.println("Result: " + result);
			break;
		case "*":
			result = calculator.multiply(a, b);
			System.out.println("Result: " + result);
			break;
		case "/":

			result = calculator.divide(a, b);
			System.out.println("Result: " + result);
			break;
		default:
			System.out.println("Invalid operation!");

			scan.close();

		}

	}

	static double add(double a, double b) {
		return a + b;
	}

	static double subtract(double a, double b) {
		return a - b;
	}

	static double multiply(double a, double b) {
		return a * b;
	}

	static double divide(double a, double b) {
		return a / b;
	}

}
