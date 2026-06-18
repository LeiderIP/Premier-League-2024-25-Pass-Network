# Premier League 2024/25 — Pass Network Explorer

Interactive pass network visualisation for any match in the 2024/25 Premier League season, built from StatsBomb event data.

![Python](https://img.shields.io/badge/Python-3.10+-blue?style=flat-square&logo=python) ![SVG](https://img.shields.io/badge/Viz-SVG%20%2B%20JS-orange?style=flat-square) ![Data](https://img.shields.io/badge/Data-StatsBomb-red?style=flat-square)

---

## Live Demo

**[Open Pass Network Explorer](https://leiderip.github.io/Premier-League-2024-25-Pass-Network/Pass_Network.html)**

---

## Features

- Select any of the 380 matches and either team
- **Nodes** positioned at each starter's average pass location — reflects real tactical role
- **Node size** scales with pass involvement
- **Edge thickness** scales with pass frequency between two players
- Network **frozen at the first substitution** — standard pass network convention
- Hover any node or edge for exact stats
- Jersey numbers shown inside each node
- **Dark / Light theme toggle**

---

## Method

Only **completed passes between starting XI players**, before either team makes its first substitution, are included — this is the standard methodology used in professional pass network analysis, since substitutions break the original tactical shape.

Average position is computed from each player's pass origin locations during that window, giving a more accurate picture of real positioning than nominal formation slots.

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
