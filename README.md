# Frogger

YouTube Demo Link: https://youtu.be/5EHK2Ya0CcE

Inspired by the classic arcade game frogger, the player controls the frog using pushbuttons and accumulates points by moving forward. This design features a double buffer system in both the pixel and text buffers to eliminate buffer flickering on screen refresh. It also includes a custom startup sound and event-triggered sound effects. 

To play, navigate to https://cpulator.01xz.net/?sys=arm-de1soc and paste all code from Frogger_final.s into the editing window. Press "Compile and Load" scroll down in the devices panel until the vga pixel buffer device tab is visible. This is where the graphics for the game are displayed. For easier gameplay, the pushbuttons device tab can be dragged down to meet the vga pixel buffer and the size of the pixel buffer can be increased by clicking the down arrow at the top left corner of the device tab.

<img width="500" alt="Screenshot 2024-10-23 at 11 24 53 PM" src="https://github.com/user-attachments/assets/57c7ca49-548a-46e0-b8bd-1d3b77440d0f">

Image of gameplay run on cpulator

#

### Controls
Button #0: Move frog right

Button #1: Move frog left

Button #2: Move frog down

Button #3: Move frog up

Note: Buttons must be unchecked before use. Unchecking a checked button will not move the frog. The frog can only be moved by checking an unchecked button.

### Scoring system
Increment score by ten when frog moves forward, moving backwards and forwards again does not count. Points only accumulate when the frog moves to a previously unreached y-coordinate.

Powerup #1 (pink square) adds one life when collected

Powerup #2 (yellow square) adds 100 points when collected

Evil powerup (red square) subtracts 100 points when hit.
