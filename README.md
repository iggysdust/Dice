# Dice
import java.util.Random;
import java.util.Scanner;
public class rollinDice
{
    public static void main(String[] args)
    {
    Scanner input = new Scanner (System.in);
    System.out.println("Attacker please enter your number of dice");
    int ATKdice=input.nextInt();

    Random dice1 = new Random();
    Random dice2 = new Random();
    Random dice3 = new Random();
    Random dice4 = new Random();



    int result1 = dice1.nextInt(6) +1;
    int result2 = dice2.nextInt(6) +1;
    int result3 = dice3.nextInt(6) +1;
    int result4 = dice4.nextInt(6) +1;


    System.out.println("Attack Rolls:");
    if (ATKdice==1)
    {
        System.out.println (result1);    
    } else if (ATKdice==2) 
    {
        System.out.println (result1+"    "+result2);    
    } else if (ATKdice==3) 
    {
        System.out.println (result1+"    "+result2+"    "+result3);    
    }
    else if (ATKdice==4) 
    {
        System.out.println (result1+"    "+result2+"    "+result3+"    "+result4);    
    }
    
    }
}
