---

## Zombie Shooter Prototype

### 🔫 Zombie Shooter Prototype 🎮

This is a zombie shooter game prototype developed using **Unreal Engine 5.4**.

### 📖 Purpose of the Prototype

The primary purpose of this prototype was to explore and implement the features of the Unreal Engine 5 **First Person Template**.

* **Experiment/Hypothesis**: The goal was to verify that a basic zombie shooter game, including player movement, shooting mechanics, and simple enemy AI, could be built efficiently using the First Person Template as a foundation. The hypothesis was that this template would significantly reduce development time for core mechanics, allowing for a focus on specific game logic.

* **Outcome**: This purpose was successfully achieved. The First Person Template provided a solid base for character control and input, which allowed for a quick implementation of the core gameplay loop.

* **Planned Duration**: 2 days
* **Actual Duration**: 2 days

* **Trial and Error**: In the process of making the continuous fire function work, there was an initial challenge because of an Unreal Engine version change. The shooting logic, which used to be in the **`BP_FirstPersonCharacter`**, had been moved to the **`BP_Weapon_Component`**. This made it difficult to follow older tutorials. However, by understanding the underlying principles, I was ultimately able to implement the desired continuous fire feature.

### ⌨️ Controls

The player can be controlled using the following keys:

* **Move**: `WASD`
* **Jump**: `Spacebar`
* **Shoot**: `Mouse Click` (Hold for continuous fire)
* **Reload**: `R`

### 🧠 Useful Knowledge Gained

* **Efficient Input Handling**: Implementing continuous fire was a challenge with `Delay` nodes. I used **`Set Timer by Event`** to start a timer on mouse click and clear it on release, which allowed for a clean and reliable continuous fire system. This experience taught me that `Set Timer by Event` is a powerful tool for controlling precise, time-based logic beyond simple delays.

### 💡 Potential Enhancements

While this prototype successfully implements the core mechanics, here are several features that could be added to expand it into a more complete game:

* **Different Zombie Types**: Introducing different types of zombies with unique behaviors and abilities, such as a fast runner or a tanky brute.
* **Advanced Weapon System**: Implementing various types of weapons with different stats, such as damage, fire rate, and reload speed.
* **Score and Wave System**: A system that tracks the player's score and spawns more zombies as the player survives for longer periods.
* **Power-ups**: Introducing power-ups that temporarily boost the player's abilities, such as a temporary damage increase or a health pack.
