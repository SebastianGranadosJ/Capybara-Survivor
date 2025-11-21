# 🐹 **Capybara Survivor**
A roguelike **Vampire Survivor–style** game built in **Godot**, featuring an adaptive difficulty system powered by **numerical analysis and linear regression**.

🎮 **Play here:**  
👉 https://daniel555as.github.io/CapybaraSurvivor/

---

## 📘 **About the Project**
This project was developed as part of a **Numerical Analysis** course, with the goal of applying a numerical method to a fully functional videogame.  
The chosen method is **Linear Regression**, used to dynamically adjust game difficulty based on player performance.

Capybara Survivor is a survival roguelike where continuous waves of enemies attack the player. Defeating enemies grants **experience**, enabling the player to **level up** and obtain new **weapons** or **items**.

After **5 minutes** of survival, the **Boss Slime** appears. Defeat it to win.

---

## 🔢 **Numerical Method: Linear Regression–Based Difficulty System**
The core academic purpose of this project is to integrate a numerical method into game mechanics.  
The game uses **Linear Regression** to build an **adaptive difficulty curve**:

1. The system records the player's **Score** every **10 seconds**.  
   - Score increases when killing enemies, leveling up, or obtaining weapons.

2. After **5 score samples**, a **linear regression** is computed:  
   - **X-axis:** time  
   - **Y-axis:** score  

3. The resulting **slope** reflects how fast the player is progressing.

4. **Difficulty updates occur every 40 seconds**, using the most recent regression slope:  
   - **High slope:** player is progressing too fast → difficulty increases more  
   - **Low slope:** slow progression → mild or no difficulty increase  

This creates a **mathematically driven dynamic difficulty system** instead of static tuning.

---

## 🛡️ **Gameplay Features**

### **Weapons (3 total)**
- **Arrows** – Fast directional projectiles  
- **Magic Area** – Circular AoE attack  
- **Shurikens** – Rotating blades around the player  

### **Items (5 total)**
Items improve various stats such as movement speed, damage, attack rate, or area.

### **Core Mechanics**
- Continuous enemy waves  
- Experience and level-up system  
- Randomized upgrades  
- Difficulty scaling every 40s via regression slope  
- Final boss at 5 minutes  

---

## 🧪 **Technology Stack**
- **Engine:** Godot  
- **Language:** GDScript  
- **Math:** Linear Regression for difficulty scaling  

---

## 🚀 **How to Play**
Play instantly in your browser:  
👉 https://daniel555as.github.io/CapybaraSurvivor/

Move, survive, level up, defeat enemies, and ultimately confront the Boss Slime.  
Your score growth shapes the challenge level—literally.

---

## 🏁 **Final Notes**
The project demonstrates how **numerical methods**, such as linear regression, can be meaningfully integrated into game design to create adaptive systems like progressive difficulty scaling.

Enjoy your survival journey with the capybara! 🐹🔥
