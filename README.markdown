# Virtual Pet Simulator

## Project Overview
This is a web-based Virtual Pet Simulator developed as part of the Unified Mentor Internship Program. The application allows users to care for a virtual pet by feeding, playing, and putting it to sleep, with attributes (hunger, happiness, energy) displayed via progress bars. The pet’s state is reflected through emoji changes and CSS animations, built using HTML, Tailwind CSS, and JavaScript.

### Technologies Used
- **HTML**: Structures the pet display, progress bars, and interaction buttons.
- **Tailwind CSS**: Provides responsive styling via CDN.
- **CSS**: Custom animations for pet states (happy, hungry, sleeping).
- **JavaScript**: Manages pet attributes, real-time updates, and user interactions.

### Features
- **Interactive Pet**: Users can feed, play, or put the pet to sleep, affecting hunger, happiness, and energy.
- **Real-Time Updates**: Attributes decay every 5 seconds when awake, with progress bars reflecting changes.
- **Visual Animations**: The pet’s emoji changes (e.g., 😴 for sleeping, 😣 for hungry) with animations (bouncing, shaking, sleeping).
- **Responsive Design**: Adapts to desktop and mobile screens using Tailwind CSS.
- **Status Messages**: Displays the pet’s state (e.g., "Your pet is happy!").
- **Sleep Mode**: Disables interactions while the pet sleeps, restoring energy.

### Setup Instructions
1. **Clone the Repository**:
   ```bash
   git clone <repository-link>
   ```
2. **Navigate to the Project Directory**:
   ```bash
   cd virtual-pet-simulator
   ```
3. **Open the Application**:
   - Open `index.html` in a web browser (e.g., Chrome, Firefox).
   - No additional dependencies are required, as Tailwind CSS is loaded via CDN.

### How to Use
1. **Interact with the Pet**:
   - **Feed**: Click "Feed" to increase hunger (+20) and happiness (+10), but decrease energy (-5).
   - **Play**: Click "Play" to increase happiness (+20), but decrease hunger (-10) and energy (-15).
   - **Sleep**: Click "Sleep" to toggle sleep mode, restoring energy (+5 every 5 seconds) but decreasing hunger (-1). Interactions are disabled during sleep.
2. **Monitor Attributes**:
   - Progress bars show hunger, happiness, and energy levels (0-100).
   - Attributes decay every 5 seconds when the pet is awake (hunger -2, happiness -1, energy -1).
3. **Pet Status**:
   - The pet’s emoji and animations change based on its state (e.g., hungry if hunger < 30, happy if happiness > 70, sleeping).
   - Status messages update in real-time (e.g., "Your pet is hungry!").

### Project Structure
```
virtual-pet-simulator/
├── index.html      # Main HTML file for the pet simulator
├── style.css       # Custom CSS for pet animations
├── script.js       # JavaScript for game logic and attribute updates
└── README.md       # Project documentation
```

### Code Quality
- **Modular**: Separate functions for updating bars, pet status, and handling interactions.
- **Safe**: Prevents interactions during sleep and ensures attribute bounds (0-100).
- **Testable**: Attribute update logic is isolated for potential unit testing.
- **Maintainable**: Clear variable names, comments, and organized code.
- **Portable**: Runs in any modern browser with only Tailwind CSS CDN dependency.



