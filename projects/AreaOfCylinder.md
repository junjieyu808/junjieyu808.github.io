---
layout: project
type: project
image: img/Cylinder.jpg
title: "Simple Cylinder Calculator"
date: 2022
published: true
labels:
  - Java
  - jGRASP
summary: "A program I had done in ICS 111 which will create a simple cylinder calculator"
---

This is a program I had done in ICS 111 which will create a simple cylinder calculator where it will ask the user for a 
radius and the height of the cylinder. Then it will calculate the area of the cylinder.


```cpp
import java.util.Scanner;
/**
* A program that calculate the area of cylinder that input from the user.
* @author Junjie Yu
* @since 9/16/22
*/
public class AreaOfACylinderJunjieYu {
   /**
   * main method.
   * @param args not used.
   */
   public static void main(String[] args) {
      //declare and initialize Scanner to read keyboard
      Scanner userIn = new Scanner(System.in);
      String sTemp = "";
      //declare h, r, and a variable for height, radius, and area
      double h, r, a;
      //declare pi as a static constant variable
      final double pi = 3.14159;
      
      //get input from the user
      System.out.println("Please enter the radius of your cylinder:");
      sTemp = userIn.nextLine();
      //convert string to a double number
      r = Double.parseDouble(sTemp);
      //show the user what number had entered
      System.out.println("You entered a radius of: " + r);
      
      //get input from the user
      System.out.println("Please enter the height of your cylinder:");
      sTemp = userIn.nextLine();
      //convert string to a double number
      h = Double.parseDouble(sTemp);
      //show the user what number had entered
      System.out.println("You entered a radius of: " + h);
      
      //calculate the area and show the user
      a = 2 * pi * r * (h + r);
      System.out.print("The area of a cylinder of radius " + r + " and height " + h + " is ");
      //use String.format "%.2f" to format the area to 2 decimal
      System.out.print(String.format("%.2f", a));
      
         
   } //closes main method

} //closes class
```
