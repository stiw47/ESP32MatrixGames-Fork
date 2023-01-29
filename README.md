### ESP32Matrix (original README from original repo):
*ESP32 code to run on a 16x16 WS2812B matrix with Tetris, Snake, Breakout and Bluetooth control via an Android app.
See this youtube video for more information: https://www.youtube.com/watch?v=apmOSQmeKJA*

Original github repo: https://github.com/s-marley/ESP32Matrix

# ESP32MatrixGames PS4 Controller Fork
This is my fork of s-marley's great software. My wish was to play these great old-school games on my DIY WS2812B 16x16 matrix, with PS4 controller, not via touch screen, so I adjusted code to my needs and added support for PS4 controller.

## Credits
* Most of the credits are going to [s-marley](https://github.com/s-marley), since he wrote the code for the games, and his repo I forked.
* Not less important, credits to  [un0038998](https://github.com/un0038998). On his [repo](https://github.com/un0038998/PS4Controller_ESP32) I learnt how to use PS4 controller in Arduino IDE. 
* At the end, thanks [aed3](https://github.com/aed3) for [PS4-esp32 library](https://github.com/aed3/PS4-esp32), and [Aaron Liddiment](https://github.com/AaronLiddiment) for [LEDMatrix](https://github.com/AaronLiddiment/LEDMatrix), [LEDText](https://github.com/AaronLiddiment/LEDText) and [LEDSprites](https://github.com/AaronLiddiment/LEDSprites) libraries.

## Usage
1. I assume that you already have (or made) some 16x16 matrix and that you know to connect it. If not, then watch [first s-marley's (great) video](https://www.youtube.com/watch?v=_0a9JZLGu4M).
2. Please use v1.0.6 of ESP32 boards in Arduino IDE. In my case, it wont compile with v2.0.0 and above
3. Regarding LEDMatrix, LEDText, LEDSprites and PS4 libraries - there will be needed some slightly modifications. Watch [s-marley's second video](https://www.youtube.com/watch?v=cqmWfE1DSyM) for LED libraries and [un0038998's video](https://www.youtube.com/watch?v=dRysvxQfVDw) for PS4 library.
4. Connect your ESP32 board to Arduino IDE and upload the sketch. Connect GPIO0 from ESP32 to data line on matrix (or change GPIO0 in code to fit your need)

## Controls
* Left, Right, Down, Up (Analog not implemented)
* Circle - Rotation in Tetris
* Cross - Enter the game // choose the menu item
* Options - Exit to menu when in game
* Restart game from score screen - any of: Left, Right, Down, Up, Circle, Cross, Square, Triangle
* You can scroll through Pixel Art with Left, Right (or you can wait auto-scroll)

Planning to add more Pixel Art
