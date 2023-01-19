---
layout: project
type: project
image: img/pokePVP/pokebattle.png
title: "Pokemon PvP"
date: 2021
published: true
labels:
  - Java
  - text based
  - jGrasp
summary: "My team and I developed a text based game that emulates the combat system of Pokemon."
---

<div class="text-center p-4">
  <img width="350px" src="../img/pokePVP/pokePvP.png" class="img-thumbnail" >
</div>

## What is Pokemon PvP

Pokemon is a popular media franchise centered around fictional creatures called "Pokemon", which humans, known as Pokemon Trainers, catch and train to battle each other for sport. Our goal is to create a text-based implementation of the Pokemon battle system using Java. Our program boasts an authentic battle system that closely simulates the gameplay mechanics of the classic Pokemon games. The game was divided into three phases: Game Setup, Battling, and Game Over. In the first phase, players will choose one Pokemon to battle with and the program will randomly choose which player goes first. In the second phase, the two players will alternate turns, entering commands to attack until one Pokemon "faints" (reaches 0 HP). The players will have the option to perform fast attack, special attack, or pass to build energy. A player must "pass" at least three times in order to build up energy for a special attack. In the final phase, once a player's Pokemon has fainted, the game will end and a congratulatory message will be printed to the winner. 

## Responsibilities and Lessons

As the lead programmer for this project, my role entailed the development of key components such as player creation, pokemon selection, and the main battle loop. To begin, I collaborated with my team members to establish a comprehensive project design and subsequently assigned tasks based on individual strengths and availability. or my portion of the work, I started by constructing the necessary player and pokemon objects, which served as the foundation for the program. Subsequently, I implemented the overall structure for the three battle phases, providing clear guidelines for my team members to efficiently integrate their contributions. Once completed, I focused on the implementation of the player creation, pokemon selection, and main battle loop. As the project progressed, it was my responsibility to consolidate the various components into a seamless and cohesive program.

This project not only served as a valuable opportunity to solidify my understanding of Java, but also provided me with invaluable experience in collaborating with others on a shared project. I am proud of the final outcome and the skills and knowledge I have gained through this experience.

## Sample Code

Here is some code of a helper function that offers players the choice to reselect their pokemon if they so choose so:

```java
 public static Pokemon reChoose(Pokemon p) {
      
      boolean reChoose = true;
      String yesNo = "";
      Pokemon poke = p;
      Scanner userIn = new Scanner(System.in);
      
      while (reChoose) {
         System.out.println("Would you like to reroll your pokemon? Y/N");
         yesNo = userIn.nextLine();
         yesNo = yesNo.toUpperCase().trim();
         
         // Switch based on player's choise
         switch (yesNo) {
            case "Y": //Reroll Pokemon
               poke = choosePokemon(); 
               System.out.println(poke);          
               break;
            case "N": //Keep Pokemon
               reChoose = false;
               break;
            default: //Invalid choice
               System.out.println("\n=======Invalid Menu Choice=======");
               System.out.println("Please enter Y/N");
               System.out.println("=================================\n");
               break;
         } // Closes Switch
      } // Closes while loop
      return poke;
}
```


Source : [GitHub](https://github.com/LuuDanny/Pokemon-PvP).
