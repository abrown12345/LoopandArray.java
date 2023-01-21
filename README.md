# LoopsandArray.java
import java.util.Scanner;
import java.util.ArrayList;
import java.util.Collections;
import java.util.List; 
public class loopAndMap {

	public static void main(String[] args) {
		Scanner input= new Scanner(System.in);
		List<Double> numbers= new ArrayList<>(); 
		
		for(int i=0; i<5; i++) {
			System.out.println("Enter a number:");
			numbers.add(Double.parseDouble(input.nextLine())); 
		}

		System.out.println(numbers);
		double sum=0.0; 
		double product= 1.0; 
		for(int i=0; i<numbers.size(); i++) {
			sum +=numbers.get(i);
			product *= numbers.get(i);
		}
		System.out.printf("Sum: %f Product: %f\n", sum, product);
		Collections.sort(numbers);
		System.out.printf("Largest: %f Smallest: %f\n",(numbers.get(numbers.size()-1)), numbers.get(0));
	}

}
