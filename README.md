Keypad Sequence: An Event Puzzle Game
A sleek, professional, and high-stakes puzzle game designed for live events, escape rooms, or team-building challenges. Players must use a physical reference sheet to decipher the correct sequence of symbols on a futuristic digital keypad—all against a ticking clock.

Table of Contents
The Vision

Gameplay & Features

How to Play

Impact & Use Cases

Technical Details

Customization

Installation & Deployment

License

The Vision
In the world of live events and competitive gaming, engagement is everything. Keypad Sequence was born from the need for a polished, self-contained digital puzzle that could be seamlessly integrated into a physical environment. The goal was to create an experience that feels premium, tense, and incredibly satisfying to solve—transforming a simple memory task into a thrilling "bomb defusal" scenario.

This project bridges the gap between digital and physical gameplay, requiring players to interact with a real-world object (the printed key) to succeed in the digital realm.

Gameplay & Features
The game is designed to be simple to understand but challenging to master under pressure.

Core Mechanic: Players are presented with a grid of symbols. Their mission is to click them in the correct sequence, which is determined by a master list on a physical sheet provided by an event coordinator.

Progressive Difficulty: The challenge escalates through three distinct rounds, increasing the number of symbols players must remember and sequence correctly.

High-Stakes Timer: Each round has a generous but firm time limit. Failure to complete the sequence in time, or a single incorrect click, results in immediate failure and resets the game to Round 1.

Futuristic Aesthetic: A dark, neon-infused "hacker console" theme immerses the player. Glowing buttons, smooth animations, and a clean layout make the experience feel professional and engaging.

Rich Audio-Visual Feedback: Every interaction is met with a response.

Success: A satisfying chime and a screen flash.

Failure: A jarring buzzer and a "shake" animation.

Victory: A triumphant audio cue and a bold "MISSION COMPLETE" banner.

How to Play
Receive the Key: An event coordinator gives you a printed sheet containing the master sequence of all possible symbols. This sheet is your guide.

Start the Game: Click the "Start Game" button on the screen to begin Round 1.

Observe the Grid: A random selection of symbols will appear on the keypad.

Enter the Sequence: Find your current symbols on the printed sheet. Click the on-screen buttons in the order they appear on the sheet.

Beat the Clock: Successfully solve all three rounds before their respective timers expire to win the game.

Impact & Use Cases
This isn't just a game; it's an engagement tool.

Escape Rooms: An ideal digital puzzle that requires players to first find the physical "key" (the symbol sheet) elsewhere in the room.

Corporate Team-Building: Fosters communication and collaboration as one team member can read the sequence while another inputs it, testing coordination under pressure.

Live Gaming Events & Booths: A quick, replayable, and exciting attraction to draw in crowds at conventions or promotional events. It's as fun to watch as it is to play.

Technical Details
Keypad Sequence is crafted with pure, efficient web technologies, ensuring maximum compatibility and performance with no external dependencies.

Languages: Vanilla HTML, CSS, and JavaScript.

Styling: Tailwind CSS is used for its utility-first framework, enabling rapid and responsive UI development.

Fonts: Google Fonts (Orbitron and Roboto Mono) are used to achieve the distinct futuristic theme.

Audio: The Web Audio API dynamically generates all sound effects (clicks, success, fail, victory), eliminating the need for audio files and ensuring the game is a single, self-contained unit.

Customization
The game is designed to be easily modified for your specific event. You can change the symbols, the number of rounds, the symbols per round, and the timers by editing two simple arrays in the index.html file.

To change the symbols, modify the REFERENCE_ORDER array:

const REFERENCE_ORDER = ['Ω', 'ψ', 'λ', 'Φ', '★', /* ...add or remove symbols */];

To adjust the rounds, modify the ROUNDS_CONFIG array:

const ROUNDS_CONFIG = [
    //          symbols-on-screen, timer-in-seconds
    { number: 1, symbols: 4, timer: 60, gridCols: 'grid-cols-2' },
    { number: 2, symbols: 6, timer: 120, gridCols: 'grid-cols-3' },
    { number: 3, symbols: 10, timer: 180, gridCols: 'grid-cols-5' },
];

Installation & Deployment
No complex setup is required.

Local Usage: Simply download the index.html file and open it in any modern web browser.

Web Deployment: Deploy the single index.html file to any static web host, such as GitHub Pages, Vercel, or Netlify, to make it accessible online.
