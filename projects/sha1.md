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

The goal of this project was to produce an implementation of the deprecated SHA-1 (Secure Hash Algorithm 1) cryptographic hash function in C that was able to take in and encrypt text files. SHA-1, developed by the National Security Agency (NSA), was a widely adopted cryptographic hash function that was designed to take an input (or "message") and produce a fixed-size output, commonly referred to as a "hash." It was widely utilized in various security protocols and applications, such as digital signatures, software protection, and file integrity verification. However, due to recent advancements in the field of cryptography and the discovery of collision vulnerabilities, its usage has been officially deprecated by the National Institute of Standards and Technology (NIST) in 2011. Despite being considered as a broken hash function, this project aimed to demonstrate the inner workings of the algorithm and its usage for educational and research purposes.

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


Source : [GitHub](https://github.com/LuuDanny/SHA1-Implementation-in-C).
