/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */

/**
 *
 * @author Devesh
 */
public class fundo {
    int minSpeed = 1;
    int maxSpeed = 200;
    boolean isTheCarOn = false;
    String name = "Devesh";
    char conditionOfcar = 'A';
    
    public void print()
    {
        System.out.println("min speed is"+ minSpeed);
        System.out.println("Max speed is "+ maxSpeed);
        System.out.println("Is car on?"+ isTheCarOn);
        System.out.println("Car's name"+ name);
        System.out.println("Condition of car"+ conditionOfcar);
    }
    
    public fundo(int customMinSpeed, int customMaxSpeed)
    {
        minSpeed = customMinSpeed;
        maxSpeed = customMaxSpeed;
        
    }
    public void condition()
    {
        conditionOfcar = 'B';
        System.out.println("condition of car"+conditionOfcar);
    }
    public int distance()
    {
        return 200;
    }
     public static void main(String[] args)
    {
       fundo fun = new fundo(10, 500);
       System.out.println(" After custom changes in speed ");
       fun.print();
       System.out.print(" Car's condition after if travelled 200 km ");
       fun.condition();
       System.out.println("Car's has travelled "+fun.distance()+" Kms");
      
       
       
    }
    
}
