How to Play the Game:
To begin playing the game, load it up and press the start button. The player controls a dog, and movement is controlled using the arrow keys:

Arrow Up: Move forward.
Arrow Left: Move left.
Arrow Right: Move right.
Arrow Down: Move backward.
As you play, the game will display a timer in the top-left corner of the screen, and a score counter in the top-right corner. Each level gives the player a limited amount of time, but upon completing a level, the timer increases slightly to give the player more time.

The objective is to collect treat bones scattered across the level. Each treat bone collected increases the player’s score. However, the levels also contain thorn bushes that act as deadly obstacles. If the player runs into a thorn bush, they die instantly, ending the game.

Each new level will contain more treat bones to collect and more thorn bushes, making the game progressively more challenging. Occasionally, power-ups will spawn, giving the player additional time to continue playing. Power-up spawn rates vary, and they can be a helpful advantage, allowing the player to continue for longer and achieve a higher score.

The game continues as long as the player avoids thorn bushes and keeps collecting treats within the time limit. If the timer runs out or the player hits a thorn bush, the game ends.

Results of Playtesting:
During playtesting, I observed that the game runs smoothly and feels well-balanced overall. However, one area that could use improvement is the spawn rate of power-ups. As it stands, if the player gets lucky, power-ups can spawn too frequently during a level, potentially allowing the player to continuously extend their time in the game. This can make certain runs feel unbalanced in favor of players who happen to get a streak of quick power-ups.

Another issue that arose during testing was a bug where a power-up might spawn even after the player has died. While all other item spawning stops upon death, the power-up spawning can still occasionally occur, which was an unexpected result.

On the positive side, the game is enjoyable and provides a good challenge. The mechanics of avoiding the thorn bushes while racing against the timer create a fun and somewhat addictive experience. Players find themselves constantly pushing for a higher score while navigating around the increasingly dangerous thorn bushes.

Documentation of Changes Made Between Phase I and Phase II:
Added Sound Effects:

In Phase I, there were no sound effects in the game. For the final phase, sound effects were added to enhance the player's experience. These include sounds for collecting treats, hitting obstacles, and the game-over sound, providing more auditory feedback and immersion.
Changed Background Image:

The background was originally a placeholder texture. In Phase II, this was replaced with a more appropriate grass texture that better fits the theme of a dog running through a field chasing treats. This change improved the visual aesthetics of the game.
Updated Cactus to Thorn Bush Texture:

In Phase I, the obstacles were represented as cacti. For the final phase, I replaced the cactus texture with a thorn bush texture to better match the game’s theme and setting. Thorn bushes are more fitting for the environment of a dog chasing treats outdoors.
Improved Collision Spawning Logic:

One of the most important gameplay changes was made to the coin_spawn() function. Initially, there was a high chance that a thorn bush would spawn directly on top of the player when starting a new level, leading to instant death without any time to react. To address this, I added a check that ensures thorn bushes do not spawn too close to the player's starting position. This change improved fairness and reduced player frustration, making the game feel less punishing and more balanced.