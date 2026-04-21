# Final Project: Text Adventure Game

## Overview

For your final project, you will design and build a text-based adventure game in the spirit of classic interactive fiction such as [Zork](https://en.wikipedia.org/wiki/Zork). Another example that is much smaller in scope so you can see the idea is [Thy Dungeon Man](https://homestarrunner.com/dungeonman). Your game must be bigger than Thy Dungeon Man but does not have to, and **should NOT** be as big as Zork.

Your game must be written in **Java** and playable through the command line.

This project replaces the final exam and is a major portion of your course grade.

Your goal is to create a game that is fun, playable, and **complete**. Scope wisely: A finished imperfect game is better than an unfinished "would have been perfect game". 

Most importantly, you want your game to be fun!

---

# Due Date / Presentation

This project is due **Thursday, May 21 at Midnight**. Late submissions will be docked **10% per day late**.

You will present your project during our scheduled final exam time on **Friday, May 22**.

---

# Workflow Instructions

## Step 1: GitHub Repo

### Option 1: GitHub Codespaces (Recommended)

1. Click the green **Code** button on this repository
2. Select the **Codespaces** tab
3. Click **Create codespace on main**
4. Wait for the environment to build (~2 minutes the first time)
5. Start coding (you are responsible for making the structure of your project this time!)

> **Note:** If the Java extension shows errors on first load, press `Cmd+Shift+P` (Mac) or `Ctrl+Shift+P` (Windows) and run **"Developer: Reload Window"**. This is a one-time setup step.

### Option 2: Local Development

1. Accept the assignment via the GitHub Classroom link
2. Clone the repository using GitHub Desktop
3. Open the project in your IDE (VS Code, IntelliJ, or Eclipse)

---

# Deliverables

You must submit:

## 1. GitHub Repository (Required)

Your completed code must be pushed to your repository.

Make sure your latest version is uploaded before the deadline.

Your instructor must be able to access and run your game.

---

## 2. README.md / Mini Game Design Document

Complete the `README.md` file in your repository.

Projects without a complete README will receive a **10% penalty**.

Use the exact section titles below.

---

## 3. Presentation / Demonstration

You will present your game during final exam time.

Be prepared to:

- Show gameplay
- Explain your design
- Discuss challenges
- Answer questions about your code

---

# Game Requirements

Your game should include:

## World Design (Choose the Setting)

You do not have to make a fantasy game where the player is in a dungeon. (Although you can do fantasy if you want.) Choose Your Own Adventure books or D&D settings might provide some inspiration. There is nothing wrong with sticking to a fantasy / dungeon setting. Some other possible settings:

- Murder Mystery
- Spaceship
- Cave System
- Village
- Escape The Room

No matter what setting you pick, your game should have:

- Multiple locations connected by movement
- A clear setting
- A map planned in advance. Before you start coding anything, draw a map of your game to plan out all of the areas that the player can reach and how they can reach them. Think about how you might implement locked doors / blocked paths / secret passageways / hidden rooms and how the player will access those. This will help when you are coding the game.

## Understand the Genre 

This game is a text-based adventure. The game describes a situation (like a room or a setting) and then prompts the player to do something.  The game should respond to all attempted player actions with the result of the action and a further prompt, even if the action was unsuccessful. **You should play Thy Dungeon Man to see how this loop works!**

For example, if the game starts in a library, the game should describe the room and list objects in the room, including exits from the room. The player then would type something like "READ Books" and the game would say "You read a book. It was good but the ending left something to be desired." OR "You don't know how to read, silly peasant." OR "You read a book and find a secret code." and so on.

As the game programmer you have to plan what you want the player to do AND anticipate actions they might take. If the player does something you don't expect, your game needs a way to handle it. (It might be as simple as insulting the player and asking them to do something else.)

### Commands

Your game should respond to typed player input. (This is how they play the game). I have suggested some below, you may need to modify or add others depending on your design. If the player tries to do something that you haven't planned for, the game still needs to decide what to do and not crash!

- GO
- LOOK
- TAKE
- DROP
- USE
- TALK
- INVENTORY

If the player types something unexpected, the game should still respond gracefully. It is okay to have a canned response for all inputs you didn't think of. Look at the Magpie and ELIZA code in the NPC section for examples of checking user input for phrases even if it doesn't match exactly. **The game should always do something when the player enters text**. Try-catch, appropriate if-elseif-else structure, and .contains() will help you make sure that you can handle all possible player input and not break your game.

### Puzzles

Your game should have puzzles that must be solved to beat it. The puzzles must be solvable using only items and information presented in the game. It has to be possible to reach the endings, these puzzles have to have solutions. You should:

- Include at least **three puzzles**
- Each puzzle should be different in type
- Puzzles must be solvable using information or items in the game

Examples of puzzles might include:

- finding a locked door and then finding the key to that locked door
- a "trading sequence" (Person A has Item X and wants Item Y. Person B has Item Y but wants Item Z. Person C has Item Z but wants Item L, etc.)
- using a certain item the player found in a certain way
- riddles

### Endings

Your game needs an ending and it must be reachable. You should have at least two endings. Ask yourself: what is the player trying to accomplish? Find the murderer? Get the treasure? Escape the castle? Consider what success and failure look like in the context of your game. What "good" and "bad" mean here is up to you and your group and the setting / design of the game.  

- At least **two endings**
- One good ending
- One bad ending (Player death alone does not count as the bad ending.)

## NPC Interaction

Your game should have at least one NPC with extended an [dialogue tree.](https://en.wikipedia.org/wiki/Dialogue_tree) This NPC may or may not be necessary for beating the game. Other NPCs can say the same thing every time or nothing at all. (You will need to think about the puzzles and endings.) If you want to give your NPCs a little life, use the [Magpie](https://runestone.academy/ns/books/published/gssm-csc101-fs25/magpie-chatbot-lab-1.html) chatbot example code (Make sure that you still code specific goals and results into the NPC if they are part of a puzzle for beating the game.)

## Programming Expectations

Your code should demonstrate:

- Classes and Objects
- Encapsulation
- Methods
- Control Structures
- Loops
- Clean Organization
- Comments where helpful

A `Player` class is strongly recommended.

---

# README.md / Mini Game Design Document

## Title

The name of your game.

---

## Authors / Programmers

Your name (and partner name if applicable).

---

## Course / Section

---

## Date Due

---

## Date Submitted

---

# Game Overview

## High Concept

One or two sentences describing the game.

Example:

> A detective mystery where the player searches a mansion, questions suspects, and uncovers the murderer.

---

## Setting

Where does the game take place?

---

## Player Goal

What is the player trying to accomplish?

---

## Genre / Tone

Examples:

- Mystery
- Fantasy
- Sci-Fi
- Comedy
- Horror

---

# Design

## Map / World Structure

Describe the areas in the game and how they connect.

---

## Puzzles

Describe each major puzzle and how it is solved.

---

## Endings

Describe the possible endings and how they are reached.

---

## NPC Design

Describe important characters and how the player interacts with them.

---

## Game Loop

Describe the repeating cycle of play:

Explore → Gather Clues / Items → Solve Puzzle → Progress

---

# Implementation

## How to Run

Step-by-step instructions for running the game.

---

## Platform / Tools

Examples:

- Java
- VS Code
- IntelliJ
- GitHub
- GitHub Codespaces

---

## Controls / Commands

List the commands the player can use.

---

# Reflection

## Design Goals

What kind of experience did you want the player to have?

---

## Biggest Challenge

What was hardest to build?

---

## How You Solved It

How did you overcome that challenge?

---

## Development Time

Approximate total time spent.

---

## What You Learned

What did this project teach you about programming or design?

---

# Academic Integrity

## Honor Statement

I affirm that this work is my own and that I can explain the code I submitted.

Digitally sign your name.

---

## AI / Collaboration Disclosure

Describe any outside help used.

Examples:

- ChatGPT helped debug a method
- Friend playtested the game
- Tutorial used for Scanner input

Write NA if none.

---

# References

## Bibliography

List any external resources used.

---

## Resources / Tutors

Write NA if none.

---

# Grading Emphasis

Projects will be evaluated primarily on:

- Completion
- Functionality
- Creativity
- Code Quality
- Puzzle Design
- Polish
- Documentation
- Presentation
- Evidence that you understand your own code

A smaller finished game beats a giant broken kingdom.
