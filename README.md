**Housie Hub - A Modern Tambola Experience**

Housie Hub is a feature-rich, modern reimagining of the classic game of Tambola (or Housie). It was built to provide a premium, competitive, and highly interactive social gaming experience, blending classic gameplay with advanced web technologies and a polished, professional design.

Live Demo: https://bbc741df-8ab4-46ad-b584-1fe8bac17a1e-00-1b05esa6fiewa.worf.replit.dev/
Video Demo: https://drive.google.com/file/d/13j7gCs0gNWONOOFHVEeS9gIqhYW1x_lD/view?usp=sharing

✨ _**Core Features**_
Housie Hub is more than just a game; it's a complete gaming platform with distinct modes, interactive elements, and social features.

**1. Three Distinct Game Modes**
The platform offers three unique ways to play, each with its own mechanics and prize structure:

Classic Mode ($100 Prize): The traditional experience with manual number calling and automatic ticket daubing.

Speed Mode ($200 Prize): A fast-paced mode featuring automatic number calling at set intervals, requiring players to manually mark their tickets.

Tournament Mode (Custom Prize Pool): A competitive mode where hosts can set the prize pool, time limit, and number of players (2-50) via a setup popup. This mode features manual calling and manual ticket marking.

**2. Advanced Gameplay Mechanics**
Dynamic & Unique Ticket Generation: Every game generates random 9x3 Tambola tickets with a guarantee of no duplicate numbers within a single ticket.

Ticket Management: Players can add new tickets during a game and remove unwanted tickets in any mode. Tournament mode includes smart player limits, preventing more tickets than players and providing a clear notification.

Bulk Number Drawing: In Classic and Tournament modes, players can choose to draw multiple numbers (1-10) at once, which are then displayed sequentially with smooth animations.

Win Detection & Celebration: The system automatically detects when a ticket has achieved a "full house" and triggers a celebratory popup announcing the winning ticket and the prize amount.

**3. Polished UI & Fluid Animations**
Professional Design System: The entire application uses a consistent design language, featuring authentic color palette and clean typography.

Initial Splash & Entrance Animations: The app greets users with a full-screen splash animation featuring an expanding gold circle, followed by a cascading "flip-in" entrance for the game columns.

"Money Shot" Auto-Daubing: The standout animation where a called number on a ticket is marked with a beautiful gold ripple effect that smoothly fills the cell.

Interactive Micro-interactions: Every element is designed to be interactive:

3D Hover Effects: Tickets lift and tilt on hover.

Button Feedback: Buttons provide satisfying press-down and lift effects.

Animated Background: A continuous, subtle ripple effect inspired by 14islands.com provides a dynamic atmosphere.

Voice Announcements: An immersive feature that announces each drawn number out loud. This can be toggled on or off by the player in all game modes.

**4. Social & Engagement Features**
Live Game Chat: All game modes include a real-time chat box where players can communicate. The chat supports timestamps, distinct usernames for each mode, and system announcements. The chat box is minimizable for an unobstructed view.

Points System: Players are rewarded with points for in-game actions to encourage engagement:

Drawing numbers (5-10 points depending on mode)

Adding new tickets (20 points)

Sending chat messages (1 point)

Winning a game (100 bonus points)

A floating points counter is always visible in the top-right corner.

**5. Seamless Navigation & Routing**
Multi-Page Experience: The application is split into a landing page (/) and a dedicated game page (/game), providing a structured user flow.

Clickable Logo: The "Housie Hub" logo always serves as a reliable link back to the main landing page.

Logical Flow: "Play Now" and "Start Playing" buttons intelligently direct users to the game modes, while links on the game page navigate back to the relevant sections on the landing page.

🛠️ _**Technologies Used**_
Frontend: React, TypeScript, Tailwind CSS

Animations: Advanced CSS (Transitions, Transforms, Keyframes)

State Management: React Hooks (useState, useEffect)

Voice Synthesis: Web Speech API

Data Storage: In-memory storage for chat and game state during a session.

🚀 **How to Run Locally**
Clone the repository:

Bash

_git clone https://github.com/your-username/housie-hub.git_
Navigate to the project directory and install dependencies:

Bash

_cd housie-hub
npm install_

Start the development server:

Bash

_npm start_
The application will be available at http://localhost:3000
