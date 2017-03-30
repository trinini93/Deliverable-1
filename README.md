# Deliverable-1
Java Bootcamp - April 2017

package com.jetbrains;

import java.util.Scanner;

public class Main {

    public static void main(String[] args) {

        Scanner scanner = new Scanner(System.in); // this will allow user to input numbers

        System.out.println("Enter numbers to reverse: "); //directions for user

        int original = scanner.nextInt(); // this will allow user's number to be assigned to the original variable
        int reverse = 0; //initially, the reverse is 0 since there is no initial reverse variable
        int remainder; // remainder will help us reverse the number


        while (original != 0) { //this will "loop" until the original == to 0

            remainder = original % 10; // original value will be divided by 10, then it's remainder will be assigned to the remainder variable
            reverse = reverse * 10 + remainder; //with the reverse initially being 0, we will multiply it by 10, then add that to whatever the remainder was. The new number will then be assigned to the reverse variable
            original = original / 10; //then, we go back to the first loop. Whatever userInput is (original variable) will be % by 10. This will keep looping until original == 0


        }

        System.out.println("Reverse numbers are: " + reverse); //this will calculate user's reverse numbers


    }
}
