[README.md](https://github.com/user-attachments/files/33116194/README.md)
# DUEL STAR IMPACT 🎴

A 2D card-collecting and battle game built with **Python** and **Pygame**, created as a term project for the **Programming** course (Section 1-2), Chulalongkorn University, 2024.

Players earn coins, roll a gacha to collect anime-style character cards, build a deck, and battle against a bot opponent.

## Features

- **Gacha system** — single and 10× rolls with rarity tiers (Common 60%, Rare 25%, Epic 10%, Legendary 4%, Limited 1%)
- **Card collection** — paged gallery of every card the player has unlocked
- **Deck builder** — choose and rearrange the cards you take into battle; decks are saved between sessions
- **Turn-based battle vs. bot** — both sides start with 3,000 HP and play cards onto four field slots; cards fight by power
- **Magic cards** — special cards (Heal, DarkHole) with effects beyond normal attacks
- **Coin & redeem-code system** to earn currency for rolling
- Win/lose end screen, animated menus, and background music

## My Contributions

I ([@RinZoKuTH](https://github.com/RinZoKuTH), committed as PunnSr) was mainly responsible for the **battle system**:

- Designed and implemented the battle logic in `battle_system.py` — player/bot state, the four-slot field, card placement and attack resolution
- Added the **magic card system** (Heal / DarkHole effects)
- Fixed the HP calculation bug and built the end-game screen
- Integrated and debugged the battle flow inside `main.py`

## Team

Developed by **MATHCOMCU32**.

| GitHub | Main responsibilities |
| --- | --- |
| [@RinZoKuTH](https://github.com/RinZoKuTH) | Battle system, magic cards, end screen, bug fixes |
| [@kluayclubaa](https://github.com/kluayclubaa) | Gacha, coin & code system, deck builder, collection, UI |

Originally developed in [kluayclubaa/GAME-PROJECT](https://github.com/kluayclubaa/GAME-PROJECT); this repository is a copy with the full commit history.

## Tech Stack

- Python 3.11+
- Pygame

## How to Run

```bash
git clone https://github.com/RinZoKuTH/GAME-PROJECT.git
cd GAME-PROJECT/pygame-cardtest
pip install pygame
python main.py
```

> **Note:** Run the game from inside the `pygame-cardtest` folder, since assets are loaded with relative paths. The project was developed and tested on **Windows**.

## Project Structure

```
pygame-cardtest/
├── main.py            # Game loop, menus, screens
├── battle_system.py   # Battle logic: players, bot, fields, magic cards
├── gacha.py           # Card definitions and gacha roll rates
├── deck.py            # Deck builder
├── button.py          # Reusable UI button
├── card/ collection/ showcaracter/   # Card artwork
├── background/ gacha background/     # Backgrounds
└── music/             # Background music
```
