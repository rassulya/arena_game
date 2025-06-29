# Arena_game

### Homework Assignment: OOP Battle Arena Game

**Objective:** To independently design and implement a program using the core principles of Object-Oriented Programming (OOP), and to practice the fundamentals of unit testing.

**Final Product:** A console-based, text-only game where two creatures fight in a turn-based battle, accompanied by a suite of tests to verify core logic.

#### Technical Specification

You are to create a program that simulates a battle between two creatures. One creature is controlled by the player, and the other is controlled by the computer. You have to follow the following rules, but you are welcome to add more functionality to the game

**Core Implementation Requirements:**

1.  **Use of OOP:** Your program must be built on OOP principles. The correct application of encapsulation, inheritance, and polymorphism is mandatory.

2.  **Class Structure:** Your project must include at least the following classes:
    * **`Creature`:** A base parent class. It must define the common attributes (e.g., health, attack power, defense) and behaviors (e.g., attack, take damage) for all combat units.
    * **Derived Classes (minimum 2):** Unique creature types inheriting from `Creature` (e.g., `Warrior`, `Mage`, `Archer`, `Ogre`, etc.). These classes must have their own unique features.
    * **`Arena`:** A class responsible for the combat process. It should take two combatants and manage the flow of the battle until a winner is determined.
    * **`Game`:** The main class that initializes and runs the game, including character selection and starting the battle in the `Arena`.

3.  **Application of OOP Principles:**
    * **Encapsulation:** All class attributes must be encapsulated. State changes to objects should only be performed through public methods.
    * **Inheritance:** Specific creature classes must inherit common logic from the base `Creature` class.
    * **Polymorphism:** Behavior must differ depending on the object's type. For example, the `attack()` method for a `Warrior` and a `Mage` should work differently (implement this through method overriding). Devise unique mechanics for each creature class.

4.  **Unit Testing:**
    * You must write unit tests to verify the core logic of your classes.
    * Your tests must cover, at a minimum:
        * The correctness of damage and health calculations in the `Creature` class.
        * The proper functioning of unique abilities in your derived classes (e.g., triggering a critical hit, ignoring defense, etc.).
        * The correct behavior of the method that checks if a creature is alive (`is_alive`).

**Game Functionality:**

* **Startup:** The game must prompt the player to select a character.
* **Opponent:** The computer's opponent should be generated automatically.
* **Battle Process:** A turn-based battle with console output detailing each turn's actions and current health stats.
* **Game End:** The game must determine a winner and display a concluding message.

**Submission Requirements:**
* Submit the source code for the project including tests (link to your github repo).
* The project and its tests must run and execute without errors.
* The code must be well-formatted and easy to understand.
