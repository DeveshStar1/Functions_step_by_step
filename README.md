/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package fundo;

/**
 *
 * @author Devesh
 */
public class Fundo {
    int maxSpeed = 100;
    int minSpeed = 0;
    boolean carOn = false;
    String carName = "dev";
    
    public void printVar()
    {
        System.out.println("max speed is ");
        System.out.println(maxSpeed);
        System.out.println("min speed is ");
        System.out.println(minSpeed);
        System.out.println("Is car on?");
        System.out.println(carOn);
        System.out.println("Car's name");
        System.out.println(carName);
    }
    public void condition()
    {
       
        carOn = true;
        
    }
    public void EngineUpgrade()
    {
        minSpeed = 0;
        maxSpeed = maxSpeed + 100;
        System.out.println("min speed is"+minSpeed);
        System.out.println("max speed upgraded to"+maxSpeed);

    }
           
   
public static void main(String[] args) {
        // TODO code application logic here
      Fundo fun = new Fundo();
      System.out.println("Initial condition for car");
      fun.printVar();
      System.out.println("During usage of car");
      fun.condition();
      fun.printVar();
      System.out.println("After Engine upgraded");
      fun.EngineUpgrade();
      fun.printVar();
      
}
    
}
