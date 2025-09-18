🚀 Space Doge - Flappy Bird Game
A fun Flappy Bird-style game featuring a space doge character navigating through obstacles in space!

🎮 Game Features
Full-screen responsive gameplay that works on both mobile and desktop
Space doge character with realistic physics and smooth animations
Live scoring system with real-time score display
Top 5 leaderboard stored in PostgreSQL database
High score celebrations with congratulations animations
No login required - anonymous gameplay with optional name entry for high scores
Space-themed graphics with scrolling star background
🛠️ Tech Stack
HTML5 - Game structure and canvas
CSS3 - Responsive styling and animations
JavaScript (Vanilla) - Game logic and mechanics
PHP - Backend API for score management
PostgreSQL - Database for leaderboard storage
📁 Project Structure
/
├── index.html          # Main game page with canvas and UI
├── style.css           # Responsive styling and animations
├── script.js           # Game logic and mechanics
├── api.php             # Backend API endpoints
├── config.php          # Database connection configuration
├── assets/
│   ├── doge-character.png  # Space doge character sprite
│   └── space-bg.jpg        # Space background image
└── README.md           # This file
🚀 How to Play
Start Game: Click the "START GAME" button on the main screen
Controls:
Desktop: Click mouse or press spacebar to make doge jump
Mobile: Tap screen to jump
Objective: Navigate through the pipe obstacles without crashing
Scoring: Each pipe you pass through increases your score
High Scores: Beat a top 5 score to enter your name on the leaderboard
🎯 Game Mechanics
Physics: Realistic gravity and jump mechanics
Difficulty: Game speed increases as your score gets higher
Collision Detection: Precise collision detection with pipes and boundaries
Particle Effects: Visual effects when jumping and crashing
Responsive Design: Automatically adapts to screen size
💾 Database Setup
The game uses PostgreSQL to store the top 5 high scores. The database table is automatically created:

CREATE TABLE high_scores (
    id SERIAL PRIMARY KEY,
    player_name VARCHAR(50) NOT NULL,
    score INTEGER NOT NULL,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
🔧 API Endpoints
GET /api.php - Retrieve top 5 scores
POST /api.php - Save new high score
🌟 Game Flow
Start Screen: Welcome screen with game title and instructions
Gameplay: Real-time action with live score tracking
Regular Game Over: Sad animation with play again button
High Score: Congratulations animation with name input for leaderboard
Leaderboard: Always visible top 5 scores in the top-left corner
🎨 Visual Features
Space theme with cosmic background
Smooth animations for character movement and UI transitions
Particle effects for enhanced visual feedback
Responsive layout that works on all screen sizes
Professional UI with glowing effects and space aesthetics
📱 Mobile Support
The game is fully optimized for mobile devices with:

Touch controls
Responsive layout adjustments
Optimized UI element sizing
Portrait and landscape support
Enjoy playing Space Doge! 🐕‍🦺🚀
