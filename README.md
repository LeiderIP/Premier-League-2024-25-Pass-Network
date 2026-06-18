# Premier League 2024/25 — Pass Network Explorer

Interactive pass network visualisation for any match in the 2024/25 Premier League season, showing how the network evolves through every substitution — built from StatsBomb event data.

![Python](https://img.shields.io/badge/Python-3.10+-blue?style=flat-square&logo=python) ![SVG](https://img.shields.io/badge/Viz-SVG%20%2B%20JS-orange?style=flat-square) ![Data](https://img.shields.io/badge/Data-StatsBomb-red?style=flat-square)

---

## Live Demo

**[Open Pass Network Explorer](https://leiderip.github.io/Premier-League-2024-25-Pass-Network/Pass_Network.html)**

---

## Features

- Select any of the 380 matches and either team
- **Phase navigation** — step through every substitution with ◀ ▶ controls, always showing exactly 11 players on the pitch
- A banner announces which player came off and which came on at each transition
- **Nodes** positioned at each player's average pass location during that specific phase — reflects real tactical role, not a fixed formation slot
- **Node size** scales with pass involvement within the phase
- **Edge thickness** scales with pass frequency between two players
- Hover any node or edge for exact stats
- Jersey numbers shown inside each node
- **Dark / Light theme toggle**

---

## Method

Each match is split into **phases bounded by lineup changes**. The Starting XI defines phase 1; every StatsBomb 'Tactical Shift' event (which fires whenever a team makes a substitution) provides the complete updated 11-man lineup with positions and jersey numbers for the next phase. This guarantees the network always reflects exactly the players on the pitch during that window — never a mix of players from before and after a substitution.

Within each phase, only **completed passes between the 11 players in that lineup** are counted. Average position is computed from each player's pass origin locations during that specific window, giving an accurate picture of real positioning rather than a nominal formation slot.

---

## Portfolio

| Project | Link |
|---|---|
| Title Race | [Live](https://leiderip.github.io/Premier-League-2024-25-Title-race/pl_position_race.html) |
| xG Race Explorer | [Live](https://leiderip.github.io/Premier-League-2024-25-xG-Title-race-/xG_Race_Explorer.html) |
| Season Shot Map | [Live](https://leiderip.github.io/Premier-League-2024-25-Shot-Map/Shot_Map.html) |
| Top Scorers vs xG | [Live](https://leiderip.github.io/Premier-League-2024-25-Top-Scorers-xG/Top_Scorers_xG.html) |
| Player Heatmap | [Live](https://leiderip.github.io/Premier-League-2024-25-Player-Heatmap/Player_Heatmap.html) |
| Scouting Radar | [Live](https://leiderip.github.io/Premier-League-2024-25-Scouting_Radar/Scouting_Radar.html) |
| Pass Network | This project |

---

*Data © StatsBomb. MSc Applied Performance Analysis — University of Essex. MIT licensed.*
