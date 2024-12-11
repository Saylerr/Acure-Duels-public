<br/>
<div align="center">
<a href="https://github.com/Saylerr/Acure-Duels-public">
<img src="images/logo.png" alt="Logo" width="80" height="80">
</a>
<h3 align="center">Acure-Duels</h3>
<p align="center">
An advanced Minecraft PVP server with a wide range of game modes, features, and possibilities. <br/>
<a href="https://www.youtube.com/@saylerek">Watch the Demo</a>
</p>
</div>

---

## About the Project
![Demo1](images/demo1.gif)

SL-Rat is a custom-built PVP server that offers unique gameplay modes. This project was created as a learning experience, combining advanced programming techniques with Minecraft’s immersive environment. It includes modes such as CS:GO, GTP, FFA, duels, party battles, events, parkour arenas, and much more.

---

## Features and Instructions

### **Arenas**
#### Creating Arenas
SL-Rat features a modern, fast temporary arena system, ensuring there are always available arenas. Temporary arenas are created 300 blocks further along the X-axis from the previous arena. To ensure proper setup, always create new arenas at x=0.

1. Create a `.schem` file using WorldEdit.
2. Place the file in `/plugins/Acure-Duels/schematics/`, or use the command:  
   `/acr arena importschematic <file name>`.
3. Generate the arena:  
   `/acr arena generate <arena name> <file name> <type (e.g., DUELS, PARKOUR)>`.
4. Set spawn points:  
   `/acr arena setlocation <arena name> <spawn1/spawn2/min/max>`.

#### Special Arenas:
- **Parkour**  
  Set the number of jumps: `/acr arena parkour setjumps <name> <count>`  
  Add finish points: `/acr arena parkour addfinishpoint`
- **FFA Event**  
  Add spawn points: `/acr arena event_ffa addspawn`

---

### **Kits**
#### Creating Kits:
1. Configure inventory using `/acr itembuilder`.
2. Create a kit: `/acr arenakit create <kit name>`.

#### Additional Options:
- **Icons:**  
  Save: `/acr arenakit saveicon <kit name>`  
  Edit and save: `/acr arenakit giveicon <kit name>`  
- **Effects:**  
  Add: `/acr arenakit addpotion <kit name> <effect> <power> <duration>`  
  Remove: `/acr arenakit removepotion <kit name> <effect>`  
- **Arena Assignment:**  
  Add arena: `/acr arenakit addarena <arena name>`  
  List assigned arenas: `/acr arenakit arenalist`.

---

### **Duels**
#### Overview:
A random duel system for 1v1 or team matches. ELO is updated globally and per kit.

#### Commands:
- **/duel <player>:** Sends a duel request.  
- **/settings:** Allows players to set the number of rounds. If players have different settings, the lower number is chosen.

---

### **Party**
#### Commands:
- **/party create:** Creates a party.  
- **/party invite:** Invites a player.  
- **/party delete:** Deletes the party.

#### Features:
The system enables team-based games and manages party leaders. Party ELO is calculated as the average ELO of all members.

---

### **Events**
#### Available Modes:
- FFA
- DeathMatch

#### Permissions:
- `acureduels.events.create`: Create events.  
- `acureduels.events.gui`: Access the event menu.

---

### **FFA**
1. Create an FFA arena.
2. Set spawn points: `/acr arena ffa setspawn`.
3. Add respawn points: `/acr arena ffa addspawnpoint`.
4. Assign a kit: `/acr arena ffa setkit`.

---

### **GTP (Game Teleport Points)**
#### Instructions:
1. Create a teleport circle: `/acr gtp create <name> <radius>`.
2. Set the center: `/acr gtp setcenterloc <name>`.
3. Add buttons: `/acr gtp addbutton <name>`.
4. Set the teleport world: `/acr gtp setworldtoteleport <name> <world>`.

#### GTP Kits:
1. Configure inventory.
2. Create a kit: `/acr gtp createkit <name>`.

---

### **ELO System and Leaderboards**
#### Leaderboards:
- Global ELO: `/top`  
- Specific kits: `%acureduels_elo_kit_top_<kit name>_<position>%`

---

### **Scoreboard**
The scoreboard dynamically adapts based on the player’s activity:
- SPAWN
- PARTY_SPAWN
- DUEL_GAME, FFA, EVENT, etc.

---

## Updates and Changelog
- New arena system implemented.  
- Added effects to kits.  
- Introduced round-based duels.  
- New FFA mode and event system (FFA, DeathMatch).

---

## Upcoming Features:
- **CS:GO Mode:**  
  - Hide enemy nicknames.  
  - DeathMatch with AI bots.  
- Party vs Party with customizable round numbers.  
- Expanded kit settings and scoreboard configurations.

---

## Contact
Have questions? Reach out on Discord: [.sayler](https://discord.com/users/448834616636211200)

