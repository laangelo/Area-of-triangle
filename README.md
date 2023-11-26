package com.triangle;

import java.util.Scanner;

public class AreaofTriangleCalculator {
public static void main(String[] args) {
AreaofTriangleCalculator calculator = new AreaofTriangleCalculator();
calculator.calculateAndDisplayArea();
    }

private double getBaseFromUser() {
Scanner scanner = new Scanner(System.in);
System.out.print("Enter the base of the triangle: ");
return scanner.nextDouble();
    }

private double getHeightFromUser() {
Scanner scanner = new Scanner(System.in);
System.out.print("Enter the height of the triangle: ");
return scanner.nextDouble();
    }

private double calculateArea(double base, double height) {
return 0.5 * base * height;
    }

private void displayArea(double area) {
System.out.println("The area of the triangle is: " + area);
    }

public void calculateAndDisplayArea() {
double base = getBaseFromUser();
double height = getHeightFromUser();
double area = calculateArea(base, height);
displayArea(area);
    }
}
