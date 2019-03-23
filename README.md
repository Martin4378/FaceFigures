# FaceFigures

import java.util.Scanner;

public class P19_FaceFigures {
    public static void main(String[] args) {

        Scanner scanner = new Scanner(System.in);

        String figure = scanner.nextLine();

        switch (figure){
            case "square":

                double squaresize = Double.parseDouble(scanner.nextLine());
                double sqface = squaresize * squaresize;
                System.out.printf("%.3f",sqface);
                break;

            case "rectangle":

                double recside1 = Double.parseDouble(scanner.nextLine());
                double recside2 = Double.parseDouble(scanner.nextLine());
                double recface = recside1 * recside2;
                System.out.printf("%.3f",recface);
                break;

            case "circle":

                double diameter = Double.parseDouble(scanner.nextLine());
                double circlearea = Math.PI * diameter * diameter;
                System.out.printf("%.3f",circlearea);
                break;

            case "triangle":

                double triside = Double.parseDouble(scanner.nextLine());
                double trihight = Double.parseDouble(scanner.nextLine());
                double triarea = (trihight * triside) / 2;
                System.out.printf("%.3f",triarea);
                break;

        }
    }
}
