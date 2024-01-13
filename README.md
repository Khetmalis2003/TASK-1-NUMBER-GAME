# TASK-1-NUMBER-GAME

import java.util.*;
class numguess {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int random = (int) (Math.random()*100)+1;
        int guess=0;
        int b=1;
        while(guess!=random){
            System.out.println(b + " Enter your guess : ");
            guess= sc.nextInt();
            if(guess==random){
                System.out.println("Your guess is correct. You guessed it in "+b +"turn");
            }
            else if(guess>random){
                System.out.println("Your guess is higher than no.");
            }
            else {
                System.out.println("Your guess is less than no.");
            }
            b++;
        }
    }
}
