---
layout: project
type: project
image: img/sha/sha1.png
title: "SHA-1"
date: 2022
published: true
labels:
  - C
  - Vim
  - SHA-1
summary: "An implemention of the NIST Secure Hash Algorithm (SHA-1) using c for the purpose of taking in and encript text files."
---

<div class="text-center p-4">
  <img width="350px" src="../img/sha/sha1.png" class="img-thumbnail" >
</div>

## What is SHA-1

Pokemon Go is a mobile game developed by Niantic, in which players use their mobile device's GPS to locate, capture, battle, and train virtual creatures called Pokemon. The objective of this project was to utilize Java in order to create a Graphical User Interface (GUI) that emulates the search and capture features of Pokemon Go in a manner reminiscent of the base Pokemon games. Additionally, the implementation of additional features such as a "Pokedex" and "Backpack" were necessary.  The Pokedex would serve as a record-keeping mechanism that maintains information pertaining to any spotted Pokemon, including the number of instances they have been either spotted or captured. The Backpack, on the other hand, would be responsible for storing information about the Pokemon that have been successfully captured, and would provide a selection of 5 different sorting options. In order to ensure scalability and flexibility, the Pokemon objects must be implemented in a manner that allows for easy addition of new Pokemon.

## Responsibilities

As the lead programmer for this project, I was tasked with the responsibility of designing and implementing the various functionalities and assets of the Graphical User Interface (GUI). To begin, I constructed a parent Pokemon class from which all other Pokemons were derived, as well as several "type" interfaces that were implemented by the Pokemons based on their specific characteristics. After creating the necessary assets for the Pokemons and their types, I moved on to conceptualizing the overall layout of the GUI through a design sketch. Utilizing the Swing library, a powerful toolkit for GUI development in Java, I crafted a visually pleasing and user-friendly interface by implementing a card layout structure that clearly separated the Pokemon, Pokedex, and Backpack features into distinct and independent fields.

## Lessons

This project presented a unique opportunity for me to expand my knowledge and expertise in the realm of Java programming, specifically in the area of graphical user interface (GUI) development. As a novice in this field, I was challenged to familiarize myself with the intricacies of utilizing the Swing library to create and manipulate various graphical elements, such as buttons, text fields, and images. Through this process, I was able to develop a comprehensive understanding of how to design and implement an elegant and user-friendly GUI. Despite the challenges I faced, I found the experience to be intellectually stimulating and immensely fulfilling. I am proud of the final outcome of this project and the skills and knowledge I have gained through this experience.

## Sample Code

Here is some code of a helper function that assits in perfroming bit-wise operations:

```java
unsigned int f(unsigned int t, unsigned int B, unsigned C, unsigned D){

    unsigned int output = 0;

    if ((0 <= t) && (t <= 19)){
        output = (B & C) | ((~B) & D);
    }
    else if ((20 <= t) && (t <= 39)){
        output = (B ^ C ^ D);
    }
    else if ((40 <= t) && (t <= 59)){
        output = (B & C) | (B & D) | (C & D);
    }
    else if ((60 <= t) && (t <= 79)){
        output = (B ^ C ^ D);
    }

    return output;
}
```


Source : [GitHub](https://github.com/LuuDanny/Pokemon-GUI).
