# School Supply Calculator (Pencils & Notebooks)

This C++ program optimizes a school supply order by calculating the most cost-effective way to purchase pencils based on bulk packaging (boxes, packs, and singles) and calculating total costs for both pencils and notebooks.

## ✏️ How it Works

The program takes a total number of pencils and breaks them down into:
- **Boxes:** 100 pencils each
- **Packs:** 20 pencils each
- **Singles:** Individual pencils remaining

It uses the **modulus operator (%)** and **integer division** to ensure you aren't buying more than you need while keeping costs low.

## 🚀 Features

- **Smart Packaging:** Automatically calculates how many full boxes and packs are needed.
- **Dynamic Pricing:** Allows the user to input current market prices for boxes, packs, singles, and notebooks.
- **Grammar Logic:** Uses conditional statements to print "box" vs "boxes" or "pack" vs "packs" based on the quantity.
- **Input Validation:** Prevents the program from crashing if a user enters a negative number or invalid character.
- **Replay Loop:** Users can run multiple calculations in one session.

## 📋 Example Output
## 💰 Supply Pricing

| Item | Packaging | Unit Price |
| :--- | :--- | :--- |
| **Pencils** | Box (100) | User Defined |
| **Pencils** | Pack (20) | User Defined |
| **Pencils** | Single | User Defined |
| **Notebooks**| Individual | User Defined |

## 🧮 Core Logic
The program uses integer division and the modulus operator to determine the most efficient packaging:

```cpp
// Logic to calculate boxes and remaining pencils
boxes = pencils / 100;
remaining = pencils % 100;
packs = remaining / 20;
single = remaining % 20;
