# Valkyria Advance

Archive repository for modified versions of the original game. Only changes introduced in this repository are documented. All other systems, enemies, mechanics and content remain unchanged from the original version.

## Play Online
 
🎮 **Play Valkyria Advance in your browser**

[https://olaelias.github.io/Valkyria-Advance/](https://olaelias.github.io/Valkyria-Advance/)

## Valkyria8 grottoppning.html

# World Map

Persistent overworld used as a hub between dungeon runs.

## Features

- Generated once and reused throughout the session.
- Built from the same room-generation system as dungeon levels.
- Contains no enemies, keys, or exits.
- Uses portals to access dungeon levels.
- Preserves its state when revisited.

## Terrain

- Grass: walkable
- Trees: blocks movement
- Mountains: blocks movement
- Water: blocks movement, allows projectiles

## Portals

Portals provide direct access to selected dungeon levels:

- Level 1
- Level 10
- Level 20
- Level 30
- Level 40
- Level 50
- Level 60
- Level 70
- Level 80
- Level 90

Entering a portal starts the corresponding dungeon level.

## Return System

Press `Q` and select the world map to leave a dungeon.

The player returns to the same portal that was used for entry.

## Generation

- Uses the existing room graph generator.
- Floor tiles become grass.
- Dungeon walls are replaced by trees, mountains, and water.
- Portals are placed on valid grass tiles.

## Purpose

Provides:

- Non-linear level selection
- A persistent overworld
- Fast travel to milestone levels
- A more open progression structure

## Valkyria5 onion.html

## Fire Onion

The Fire Onion is a floating enemy designed to provide ranged pressure from a distance.

### Behavior

The Fire Onion drifts slowly through rooms while hovering above the ground. It does not actively chase the player and instead follows a gentle wandering movement pattern. Upon detecting a player in the same room, it periodically attacks by launching fireballs.

### Fireball Attack

The Fire Onion's primary attack is a magical fireball.

The enemy briefly charges before firing, producing a visible glow around its upper leaves. Once released, the fireball travels in a straight line toward the player's predicted position. The projectile can move freely through room obstacles and remains active until colliding with a room boundary or a target.

A successful hit damages the player and produces a short burst of flame particles.

### Visual Design

The Fire Onion appears as a large onion-like creature with layered skin and oversized leaves growing from its top.

Characteristics include:

- Rounded onion body.
- Pale yellow to green coloration.
- Large leafy crown.
- Constant hovering motion.
- Subtle bobbing animation while idle.
- Bright magical glow during fireball charging.

### Gameplay Role

The Fire Onion introduces ranged combat pressure into encounters that would otherwise be dominated by melee enemies. Its purpose is to force movement, encourage positioning awareness, and punish players who remain stationary for too long.
