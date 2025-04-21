Space War 🚀
Space War is a thrilling 2D space shooter built with Python and Pygame. Pilot a spaceship, blast alien enemies, and aim for a high score! Enjoy smooth controls, collision detection, an animated GIF background, and engaging Game Over/Win states.
Features 🌟

Player Controls: Move left/right with arrow keys, fire bullets with the spacebar.
Alien Enemies: Aliens spawn randomly and descend, challenging your aim.
Bullet Mechanics: Precise collision detection for hitting aliens.
Scoring System: Score points per alien hit, win at 10 points.
Game States: "Playing," "Game Over" (alien reaches bottom), and "Win" with a fade effect.
Animated Background: Immersive GIF background powered by Pillow.
Restart Option: Press 'R' to restart after Game Over or Win.

Demo 🎮


 
Installation 🛠️
Prerequisites

Python 3.6+
Pygame (pip install pygame)
Pillow (pip install Pillow) for GIF animation

Steps

Clone the repository:
git clone https://github.com/arvindverma63/space-war.git
cd space-war


Install dependencies:
pip install -r requirements.txt

Or manually:
pip install pygame Pillow


Verify assets in assets/:

space.png (game icon)
bg.gif (animated background)
Sprites for player, alien, bullet


Run the game:
python main.py



Usage 🎯
Controls

Left Arrow: Move spaceship left
Right Arrow: Move spaceship right
Spacebar: Fire bullet
R: Restart (Game Over/Win)
Close Window: Quit

Objective

Shoot aliens to earn points.
Reach 10 points to win.
Prevent aliens from reaching the bottom to avoid Game Over.

File Structure 📂
space-war/
├── assets/                   # Images
│   ├── space.png             # Game icon
│   ├── bg.gif                # Animated background
│   └── ...                   # Player, alien, bullet sprites
├── components/               # Game logic
│   ├── player.py             # Player class
│   ├── alien.py              # Alien class
│   ├── bullet.py             # Bullet class
├── main.py                   # Main game script
├── README.md                 # Documentation
├── requirements.txt          # Dependencies
└── LICENSE                   # License file

Performance Notes ⚡

GIF Background: Large or high-frame-count GIFs (bg.gif) may slow performance. Optimize with fewer frames/resolution or use a static bg.png.
Frame Rate: Capped at 60 FPS for smooth gameplay. If bullets/aliens move slowly, adjust bullet_speed or alien_speed in components/.
FPS Monitoring: Check console for FPS output to diagnose slowdowns.

Troubleshooting 🐛

GIF Not Animating:
Verify Pillow installation (pip show Pillow).
Ensure bg.gif is an animated GIF (test in a viewer).
Check console for frame count/errors.


Slow Movement/Performance:
If FPS < 30 (see console), optimize bg.gif or switch to a static image.
Increase bullet_speed/alien_speed in components/.
Adjust bg_frame_delay in main.py (e.g., 200ms).


Missing Assets:
Confirm all images are in assets/.
Update paths in main.py if needed.



Contributing 🤝
We welcome contributions! To get started:

Fork the repository.
Create a branch: git checkout -b feature/your-feature
Commit changes: git commit -m "Add your feature"
Push: git push origin feature/your-feature
Open a Pull Request.

Include:

Change description
New dependencies/assets
Screenshots/tests for features

Future Improvements 🔮

Sound effects and music
Multiple alien waves or bosses
Power-ups and varied weapons
Customizable controls
Sprite sheet for GIF optimization

License 📜
This project is licensed under the MIT License.
Acknowledgments 🙌

Powered by Pygame and Pillow.
Inspired by classics like Space Invaders.


⭐ Love Space War? Star the repo on GitHub! Feedback and contributions are welcome. 🚀
