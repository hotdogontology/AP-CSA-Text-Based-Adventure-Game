# Final Project: Text Adventure Game

## Overview

For your final project, you will design and build a text-based adventure game in the spirit of classic interactive fiction games such as [Zork](https://en.wikipedia.org/wiki/Zork). Another example that is much smaller in scope is [Thy Dungeon Man](https://homestarrunner.com/dungeonman) (so that you can see the idea). Your game must be bigger than Thy Dungeon Man but does not have to, and **should NOT** be as big as Zork.

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

**Do not edit devcontainer.json or pom.xml. Doing so may break your project in codespaces.**

---

# Deliverables

You must submit:

## 1. GitHub Repository (Required)

Your completed code must be pushed to your repository.

Make sure your latest version is uploaded before the deadline.

Submit updates regularly! I want to see a history of you working on this project and not just one push the day before the project is due.

I must be able to access and run your game.

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

You *do not* have to make a fantasy game where the player is in a dungeon. (Although you *can* do fantasy if you want. Choose Your Own Adventure books or D&D settings might provide some inspiration in that case. There is nothing wrong with sticking to a fantasy / dungeon setting.) Some other possible settings:

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

**I suggest providing a command for the player to have the game re-describe their current location whenever they need a reminder. It's hard to remember when all you have is text!**

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

The code of your game itself must implement the following: Object Oriented Programming Principles (Class writing, Encapsulation, Objects and Methods, etc. You should have a Player Class with appropriate attribute variables. Other classes you write will depend on your game.) Write clean, organized, and well-documented (read: commented) code. Use control structures such as if-then and loops to avoid repeating yourself.

While you may use AI to assist you with this project, **you are responsible for all code submitted and may be asked to explain how any part of the code works**. If you are unable to explain a portion of the code you may be docked points.

Any of the following may be worth extra credit (not all of these are worth the same amount) if it impresses me:

-A third secret ending to the game.
-Unique mechanic. Add some game mechanic beyond just the text interaction.
-A battle system. (Maybe you are a knight or maybe you have monsters you send out like pokemon, etc)
-[Cheat Codes](https://simple.wikipedia.org/wiki/Konami_Code#:~:text=The%20Konami%20Code%20(also%20known,START%20and%2For%20SELECT%20).)
-[Easter Eggs](https://en.wikipedia.org/wiki/Easter_egg_(media)) (sometimes as simple as references or inside jokes)
-ASCII Art related to objects or NPCs or some room.
-Recursion (other than a search method in your code) 
-Use [Processing](https://processing.org/) to make a nice skin for your game. (It should still be a text-based adventure game.)
-Puzzles that are solvable but not by me.
-The rest of the class votes your game to be the best.

---

# Grading Emphasis

The rubric for grading can be found on Canvas. During our scheduled final exam time we will share and play everyone's games.

Remember! A finished "imperfect" game is better than an unfinished "it was going to be awesome" game! Keep your goals manageable and pace yourself!
