# Fantasy Battle

This is a fantasy battle game system where players fight monsters using equipment. The system calculates damage based on:

- **Equipment**: Items equipped in different slots (left hand, right hand, head, feet, chest) that provide base damage and damage modifiers
- **Stats**: Player attributes like strength that affect damage calculations
- **Armor**: Protection worn by enemies that reduces incoming damage (soak)
- **Buffs**: Modifiers that affect both damage and damage reduction

## Key Components

- **Player**: The main character that calculates damage against targets
- **SimpleEnemy**: A basic enemy type with armor and buffs
- **Equipment**: Manages items equipped in different slots
- **Inventory**: Contains the player's equipment
- **Damage**: Represents the calculated damage amount

## Damage Calculation

The damage calculation follows these steps:
1. Calculate base damage from all equipped items
2. Apply damage modifiers from items and stats
3. Calculate total damage
4. Apply soak (damage reduction) from enemy armor and buffs
5. Return final damage (cannot be negative)

