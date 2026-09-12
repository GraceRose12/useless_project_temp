<img width="1280" height="640" alt="git (1)" src="https://github.com/user-attachments/assets/8920b256-2ba8-4988-b824-5351134eb4bd" />



# [ChayaGPT] 🎯


## Basic Details
### Team Name: [Not a book]


### Team Members
- Team Lead: [Grace Rose K J] - [ICCS COLLEGE OF ENGINEERING AND MANAGEMENT]
- Member 2: [Muhsina V A] - [ICCS COLLEGE OF ENGINEERING AND MANAGEMENT]

### Project Description
[ChayaGPT is an "AI-powered" tea cooling predictor that watches your virtual cup of chaya and tells you exactly when it will slip from "perfectly sippable" to "lukewarm regret." Pour a cup, tweak the brew parameters, and watch a live simulation count down to the moment your tea is no longer worth drinking.]

### The Problem (that doesn't exist)
[Millions of cups of tea go cold every day because humans are apparently incapable of tracking basic thermodynamics while doom-scrolling. Nobody knows exactly when their chaya crosses the invisible line from "hot and comforting" to "why is this so cold."]

### The Solution (that nobody asked for)
[We deployed the full might of Newton's Law of Cooling — dressed up in flashy branding as an "AI model" — to simulate your tea's temperature in real time. ChayaGPT tracks cup type, tea volume, room temperature, and lid status, then predicts (with a very confident-looking confidence bar) exactly how many minutes you have left before your tea becomes emotionally unavailable. It even nags you with a modal popup and a pulsing "DON'T LET THE TEA DIE" button when things get dicey.]

## Technical Details
### Technologies/Components Used
For Software:
- [Languages used: HTML5, CSS3, JavaScript (ES6, vanilla — no framework)]
- [Frameworks used: None — plain HTML/CSS/JS]
- [Libraries used:Google Fonts (Baloo 2, Inter, JetBrains Mono) — loaded via CDN link, no JS libraries]
- [Tools used:Any modern web browser, VS Code (or similar) for editing]
  

For Hardware:
Not applicable — ChayaGPT is a purely software/web-based simulation project. No physical components, sensors, or hardware were used.
### Implementation
For Software:
# Installation
https://chayagptin.netlify.app

# Run
[open index.html]

### Project Documentation
For Software:

# Screenshots (Add at least 3)

(https://drive.google.com/drive/folders/1LlCcobDI7HA87lTqTc18RNAPw85KmilE?usp=sharing)

![Workflow]https://drive.google.com/drive/folders/1LlCcobDI7HA87lTqTc18RNAPw85KmilE?usp=drive_link

1. Set brew parameters
Before pouring, you configure the simulation inputs: initial tea temperature (70–98°C), room temperature (14–34°C), cup type (glass/ceramic/insulated flask), amount of tea (small/medium/large), and whether the cup has a lid. Each of these feeds into the cooling rate calculation.

2. Pour tea & start timer
Clicking "Pour Tea" resets the simulation, records a start timestamp, and locks in the cooling constant k — calculated from cup material, tea volume, and lid status (a lid multiplies k by 0.55, i.e. slows cooling).

3. Simulate cooling (Newton's Law of Cooling)
This is the actual "AI" — it's really just the classic formula:

T(t) = T_room + (T_initial − T_room) × e^(−k·t)

Every animation frame, the code computes the current simulated temperature based on elapsed time (sped up 7× for demo purposes) and this exponential decay equation.

4. Update visuals
The computed temperature drives everything visually:

The liquid height in the SVG cup
The liquid's color gradient (shifts from warm amber to cool blue-gray as it cools)
Steam opacity (fades out as it drops below ~80°C)
The live temperature readout and "time remaining" prediction with a fake confidence percentage

5. Check temperature
The app continuously checks the current temp against two thresholds: a "warning" zone (≈45°C) and a "critical" zone (≈32°C).

6a. User drinks tea
If you click "Don't Let The Tea Die" (or the modal's "Drink it now" button) before the tea goes cold, the cup tilts, the liquid drains, and you get a little "you drank the tea, respect 🫡" status.

6b. Tea expires
If you ignore it, once temperature reaches room temperature, the simulation ends with a "why is this so cold" status and a mildly judgmental modal.

It's a genuinely solid piece of interactive front-end work (SVG liquid animation, gradient interpolation, modal states) wrapped around a joke premise — which fits the "useless projects" spirit perfectly.

For Hardware:

# Schematic & Circuit
![Circuit](Add your circuit diagram here)
*Add caption explaining connections*

![Schematic](Add your schematic diagram here)
*Add caption explaining the schematic*

# Build Photos
![Components](Add photo of your components here)
*List out all components shown*

![Build](Add photos of build process here)
*Explain the build steps*

![Final](Add photo of final product here)
*Explain the final build*

### Project Demo
# Video
[Add your demo video link here]
*Explain what the video demonstrates*

# Additional Demos
[Add any extra demo materials/links]

## Team Contributions
- [Name 1]: [Specific contributions]
- [Name 2]: [Specific contributions]
- [Name 3]: [Specific contributions]

---
Made with ❤️ at TinkerHub Useless Projects 

![Static Badge](https://img.shields.io/badge/TinkerHub-24?color=%23000000&link=https%3A%2F%2Fwww.tinkerhub.org%2F)
![Static Badge](https://img.shields.io/badge/UselessProjects--26-26?link=https%3A%2F%2Ftinkerhub.org%2Fevents%2F1M8ORET9A1%2Fuseless-projects-3.0)



