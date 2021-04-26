# cbsecalc
cbse calculator
package com.company.cwp_10;

import java.util.Scanner;

public class cbse {

    public static void main(String[] args) {


        /*
Test Qustion
Write a program to Calculate percentage of a givin student in CBSE bordexam His mord from 5 student must be taken as input from the keybord
(Marks are out of 100).
*/
        Scanner scan = new Scanner(System.in);
        System.out.println("Enter your Hindi subject Marks");
        float Hindi = scan.nextFloat();
        System.out.println("Enter your Math subject Marks");
        float Math = scan.nextFloat();
        System.out.println("Enter your English subject Marks");
        float English = scan.nextFloat();
        System.out.println("Enter your Science subject Marks");
        float SST = scan.nextFloat();
        System.out.println("Enter your History subject Marks");
        float History = scan.nextFloat();

        float sum = Hindi + Math + English + SST + History;

        System.out.println("Total marks");
        System.out.println(sum);

        String yk = "You Want find your Percentage , then click 1";
        System.out.println(yk);

        int input = scan.nextInt();
        switch (input) {
            case 1:
                System.out.println("This is your %");
                float div = sum / 5;
                System.out.println(div);
                break;

            default:
                System.out.println("Out of Index");
                break;
        }
    }
}
