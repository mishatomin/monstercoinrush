# Monster Coin Rush — Game Design Document

## Overview

- **Title:** Monster Coin Rush  
- **Platform:** Android (Mobile Devices)  
- **Genre:** 2D Arcade Shooter, Endless Runner  
- **Target Audience:** Casual players aged 12–30  
- **Visual Style:** Pixel/cartoony 2D graphics  
- **Engine:** Unity (Unity Playground / Unity 2D)  
- **Language:** C#  
- **Build Target:** Android (APK)

---

## Core Gameplay

### Objective

The player must collect coins, defeat monsters, avoid damage, and survive as long as possible in an endless level.

### Controls (Touch)

- **Left Button:** Move left  
- **Right Button:** Move right  
- **Shoot Button:** Fire bullets in the facing direction  

Optional: Jump button (if verticality is implemented)

### Gameplay Loop

- The game has infinite progression.
- Monsters spawn continuously and move toward the player.
- Contact with a monster deals 0.5 HP damage.
- Player starts with 5 HP.
- Health boosts can restore HP.
- Coins are collected to increase score and can be used in the shop.

---

## Game Entities

| Entity         | Description                                |
|----------------|--------------------------------------------|
| Player         | Controllable character with 5 HP           |
| Monster        | Enemy that deals 0.5 HP damage on contact  |
| Bullet         | Fired by the player, destroys monsters     |
| Coin           | Increases score and acts as currency       |
| Health Boost   | Restores 1 HP                              |

---

## Health System

- Max HP: 5  
- Each hit from an enemy: -0.5 HP  
- Game over when HP reaches 0  
- Health can be restored by collecting boosts or via the in-game shop

---

## Combat System

- Bullets are fired in the direction the player is facing.
- Monsters are destroyed upon bullet collision.
- Enemies either patrol or move toward the player.

---

## Coin System

- Coins increase the player’s score.
- Coins can be spent on:
  - Skins
  - Health boosts
  - Power-ups

---

## UI Elements

- Virtual joystick/buttons (Left, Right, Shoot)
- Health bar (hearts)
- Coin counter
- Pause button
- Main menu with access to settings and shop

---

## Audio

- Background music (looping)
- Sound effects for:
  - Shooting
  - Monster defeat
  - Coin collection
  - Taking damage
  - Healing

---

## Monetization

- **Skins:** Purchase with coins or unlock via ads  
- **Health Boosts and Power-Ups:** Purchasable using coins  
- **Ad Integration:**  
  - Watch ads to earn coins or health  
  - Optional ad-based revive system


---

## Potential Future Features

- Additional enemy types with unique behavior
- Multiple environments/biomes
- Save system for progress
- Online leaderboards
- Co-op or PvP multiplayer
