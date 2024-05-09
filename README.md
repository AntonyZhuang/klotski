Disclaimer: 
1. This is a game that needs to be compiled on De1-Soc board using nios II processor. You will need to connect your DE1-soc Board with a PS2keyboard and a speaker to fully enjoy our game!
3. This project is developed by Antony Weihong Zhuang(me) and Yahe Zhang.

Commercial use prohibited. Plagiarism is not allowed. All rights are reserved.

contact information:
  Antony's email:
  antony.zhuang@mail.utoronto.ca
  Yahe's email:
  yahe.zhang@mail.utoronto.ca


How to operate:
To initiate gameplay or advance to the next level, simply press the enter key upon starting or completing a level. 
To navigate within the game, utilize the PS2 keyboard to select the desired block by entering its corresponding number. 
Once selected, employ the four-way arrow keys to move the block in any of the four directions (up, down, left, and right), ensuring adherence to the established Rules[1]. 
The primary objective is to move block 0 to the designated location highlighted by a red boundary. Should the need arise, pressing the space key will reset the game, allowing for a fresh start.

Rules[1]:
Like other sliding-block puzzles, several different-sized block pieces are placed inside a box, which is normally 4×5 in size. 
Among the blocks, there is a special one (usually the largest) that must be moved to a special area designated by the game board. 
The player is not allowed to remove blocks, and may only slide blocks horizontally and vertically. 
Common goals are to solve the puzzle with a minimum number of moves or in a minimum amount of time.


attribution of each teammate:

  Game Logic
  Yahe Zhang
  All the game framework and sets of rules to determine how the game operates.
  
  VGA Display
  Yahe Zhang
  -Integrate double buffering for smoother rendering.
  -Convert images into arrays and render them on the display.
  -Utilize a character buffer for printing characters on the screen.
  
  Audio (Sound Effect)
  Antony Weihong Zhuang
  
  -The functionality is achieved through a polling mechanism. Upon reaching specific milestones, which are detecting a legal movement or clearing a level, the corresponding audio samples are dynamically filled into the designated audio address.
  -Arrays of samples are employed for implementation, which are derived from sound effect .mp3 files  .
  
  
  PS2 Keyboard
  Antony Weihong Zhuang
  -The system operates through a polling mechanism. When a user inputs a valid command by pressing the keys on PS2 Keyboard, the function converts this signal into another signal from the Game Logic to advance the game.


Reference List:
[1] https://en.m.wikipedia.org/wiki/Klotski

