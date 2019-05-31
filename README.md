# Project-1
2.17 (Science: wind-chill temperature) How cold is it outside? The temperature alone is not enough to provide the answer. Other factors including wind speed, relative humidity, and sunshine play important roles in determining coldness outside. In 2001, the National Weather Service (NWS) implemented the new wind-chill temperature to measure the coldness using temperature and wind speed.
 The formula is
 
where ta is the outside temperature measured in degrees Fahrenheit and v is the speed measured in miles per hour. twc is the wind-chill temperature. The formula cannot be used for wind speeds below 2 mph or temperatures below − 58  ºF or above 41ºF. Write a program that prompts the user to enter a temperature between − 58  ºF and 41ºF and a wind speed greater than or equal to 2 and displays the wind-chill temperature. Use Math.pow(a, b) to compute v 0.16 .
CLASS NAME: Your program class should be called WindChillTemperature
Requirements:
•	use constants to store all permanent data in the formula, for example 
const double FIRST_COEFFICIENT = 35.74;
•	use variables to store data, for example 
double twc; // the wind-chill temperature
Here is a sample run:
Enter the temperature in Fahrenheit between -58°F and 41°F: 5.3 
Enter the wind speed (>=2) in miles per hour: 6 
The wind chill index is -5.56707




import java.util.Scanner;

public class CostOfDriving {
	
	public static void main(String[] args) {
		// TODO Auto-generated method stub

		Scanner input = new Scanner(System.in);

		// Prompt the user to enter the distance to drive, the fuel 
		// efficiency of the car in miles and the price per gallon.
		System.out.print("Enter the driving distace: ");
		double distace = input.nextDouble();
		System.out.print("Enter miles per gallon: ");
		double milesPerGallon = input.nextDouble();
		System.out.print("Enter price per gallon: ");
		double pricePerGallon = input.nextDouble();
		{
			input.close();
		}
		// Compute the cost of driving
		double costOfDriving = (distace / milesPerGallon) * pricePerGallon;

		// Display result
		System.out.println("The cost of driving is $" + costOfDriving);
	}
}
