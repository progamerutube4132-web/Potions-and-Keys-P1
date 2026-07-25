# 🏚️ Potions and keys P1 — Text RPG

A terminal-based text adventure built in Python. Explore a spooky mansion, collect items, avoid monsters, and escape through the Garden with the key and potion in hand.

## 🎮 How to Play

Run the game and navigate using simple text commands:

```bash
python File_Name.py
```

> Replace `File_Name.py` with your actual filename.

### Commands

| Command | Description |
|---|---|
| `go [north/south/east/west]` | Move between rooms |
| `get [item]` | Pick up the item in your current room |

Example:
```
>>> go north
>>> get key
```

## 🗺️ Map

```
         N                +-----------------+
         ^                |     Garage      |
         |                |   (Matches)     |
     W <-+-> E            +-----------------+
         |                         ^
         v                         |
         S                         |
+-----------------+       +-----------------+
|    Bathroom     | <---  |   Living Room   |
| (Poop Monster)  |       | (Toilet Cleaner)|
+-----------------+       +-----------------+
                                   ^
                                   |
+-----------------+       +-----------------+
|      Hall       | --->  |   Dining Room   |
|      (Key)      |       |    (Potion)     |
+-----------------+       +-----------------+
         |                         |
         v                         v
+-----------------+       +-----------------+
|     Kitchen     |       |     Garden      |
|    (Monster)    |       |   (Chainsaw)    |
+-----------------+       +-----------------+
                                   |
                                   v
                          +-----------------+       +-----------------+
                          |     Forest      | --->  |    Campsite     |
                          |     (Wood)      |       |  (Ice Tickler)  |
                          +-----------------+       +-----------------+
```

## 🧩 Rooms & Items

| Room | Item |
|---|---|
| Hall (start) | Key |
| Dining Room | Potion |
| Garden | Chainsaw |
| Kitchen | Monster ⚠️ |
| Living Room | Toilet Cleaner |
| Bathroom | Poop Monster ⚠️ |
| Garage | Matches |
| Forest | Firewood |
| Campsite | Ice Tickler ⚠️ |

## 🏆 Win / Lose Conditions

- **🏆 Main Win:** Reach the **Garden** while carrying both the **key** and the **potion**.
- **👹 Monster (Kitchen):** Survive only if you're carrying the **chainsaw** — otherwise, Game Over.
- **💩 Poop Monster (Bathroom):** Survive only if you're carrying the **toilet cleaner** — otherwise, Game Over.
- **🧊 Ice Tickler (Campsite):** Survive only if you're carrying **matches** and **firewood** — otherwise, Game Over.

## 🛠️ Requirements

- Python 3.x (no external libraries needed — uses only the standard library)

## 📁 Project Structure

This game is designed to run as a single script containing:
- Room/world data (`rooms` dictionary)
- Display functions (`show_instructions`, `show_status`)
- The main game loop (movement, item pickup, win/lose checks)


## 🚀 For Potions and Keys Part 2 

I will be making the game more fun by adding weapons, a health bar and a Owner that you have to defeat, and the game 
will be more randomized



## 📄 License

Open source — feel free to fork and expand the mansion!
