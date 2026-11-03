# Gridlock Authority: Director's Cut

A browser-based traffic management and incremental simulation game built with HTML5 Canvas and Vanilla JavaScript. 

## Description
You are the city's central traffic AI. Your job is to manage four major intersections, control the flow of vehicles, and prevent complete gridlock. Earn cash by getting cars safely off the screen, and use that cash to upgrade your roads, pass new city laws, and build infrastructure.

## Features
- **4 Coordinated Intersections:** Manage traffic across a 900x900 grid.
- **Dynamic Traffic Lights:** Click any intersection to manually cycle the lights (North/South <-> East/West).
- **Vehicle Variety:** 
  - *Cars:* Standard speed and payout.
  - *Trucks:* Slow, take up more space, but pay out more.
  - *Ambulances:* Fast, ignore traffic rules, and pay out massively.
- **City Laws:** Pass the "Right Turn on Red" law to speed up traffic at the risk of collisions.
- **Infrastructure:** Save up to convert an intersection into a free-flowing roundabout.
- **Gridlock Risk Meter:** Watch the risk meter. Too many waiting cars will cause a traffic jam.

## How to Play

### Controls
- **Left Click:** Click near the center of any intersection to manually change the traffic lights.
- **UI Panel:** Click the buttons on the right side of the screen to purchase upgrades and toggle laws.

### Game Loop
1. Cars spawn from the edges of the map.
2. They will stop at red lights and yield to cars in front of them.
3. You earn cash every time a vehicle successfully exits the map.
4. If cars pile up, your Gridlock Risk goes up. If it hits 100%, the city locks up.

### Upgrades
- **Traffic Flow:** Spawns cars faster so you can earn money quicker.
- **Speed Limit:** Makes all vehicles move faster.
- **Right Turn on Red (Law):** Toggleable. Allows cars to turn right even if the light is red. Fast, but risky.
- **Roundabout (Infrastructure):** Replaces the top-left intersection with a roundabout. Cars yield to cars already in the circle, reducing the need for manual light switching.

## Tech Stack
- HTML5 Canvas
- Vanilla JavaScript (No external libraries or frameworks)
- CSS3

## Local Development
No build tools required. Simply clone the repository and open `index.html` in your browser.