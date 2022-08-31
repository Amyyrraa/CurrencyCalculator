# CurrencyCalculator
My first Java Project

import java.util.*;
import java.text.DecimalFormat;
 
public class CurrencyConverter {
 
	public static void main(String[] args) {
 
		double amount, dollar,  pound, euro, yen, ringgit, rupee;
 
		DecimalFormat f = new DecimalFormat("##.##");
 
		try (Scanner sc = new Scanner(System.in)) {
			System.out.println("hi, Welcome to the Currency Converter!");

			
			System.out.println("How much Money you want to convert ?");
			amount = sc.nextFloat();
		}
 
		// For amounts Conversion
		if (amount == 0) {
			System.out.println("Invalid input");
		} else { 
			rupee = amount * 5.28;
			System.out.println("Your " + amount + " Naira is : " + f.format(rupee) + " Ruppes");
 
			pound = amount * 496.06;
			System.out.println("Your " + amount + " Naira is : " + f.format(pound) + " Pound");
 
			euro = amount * 420.72;
			System.out.println("Your " + amount + " Naira is : " + f.format(euro) + " Euro");

			dollar = amount * 450;
			System.out.println("Your " + amount + " Naira is : " + f.format(dollar) + "Dollar");
 
			yen = amount * 3.07;
			System.out.println("Your " + amount + " Naira is : " + f.format(yen) + " Yen");
 
			ringgit = amount * 94.50;
			System.out.println("Your " + amount + " Naira is : " + f.format(ringgit) + " ringgit");
		} 
		} 
		

	}
