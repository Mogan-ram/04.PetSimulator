# Virtual Pet Simulator

## Description
This is a Virtual Pet Simulator built with HTML, CSS, and JavaScript. The application allows users to interact with a virtual pet by feeding, playing, and putting it to sleep. The pet has three attributes—hunger, happiness, and energy—which are displayed as progress bars and updated in real-time based on user interactions and automatic decay over time.

## How to Run
1. Download and unzip the project files.
2. Open `index.html` in a web browser (e.g., Chrome, Firefox).
3. No additional setup is required as the project uses Tailwind CSS via CDN and vanilla JavaScript.

## How to Interact
- **Feed**: Click the "Feed" button to increase the pet's hunger and happiness, but it slightly reduces energy.
- **Play**: Click the "Play" button to increase happiness, but it reduces hunger and energy.
- **Sleep**: Click the "Sleep" button to toggle sleep mode, which restores energy but slightly reduces hunger. Interactions are disabled while the pet is sleeping.
- The pet's attributes (hunger, happiness, energy) decrease over time when awake, and the pet's appearance changes based on its state (hungry, happy, or sleeping).

## Features
- **Visual Pet**: Represented by an emoji with CSS animations to reflect its state (hungry, happy, or sleeping).
- **Interactive UI**: Clean, responsive interface styled with Tailwind CSS.
- **Real-time Updates**: Progress bars show the pet's attributes, updated every 5 seconds or after interactions.
- **Game Logic**: Attributes change based on user actions and time, with appropriate bounds (0-100).