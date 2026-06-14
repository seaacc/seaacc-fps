SeanFPS v0.9.1
==============

Small polish release for the controller-calibration build.

Files:
- index.html = the whole game in one file

What changed from v0.9:
- Cleaned up the harmless double-finish path in controller calibration.
- Documented that calibrated movement is digital/D-pad style for reliability on compact controllers.
- CAL/PAD buttons are hidden on desktop/fine-pointer layouts.
- Added keyboard shortcut C to start controller calibration on desktop.
- G or ` still toggles controller debug.

How to calibrate on iPhone:
1. Open the game.
2. Tap CAL.
3. Follow each prompt:
   - RIGHT
   - LEFT
   - UP / FORWARD
   - DOWN / BACK
   - SHOOT / A
   - OPEN / B
   - STRAFE LEFT / L
   - STRAFE RIGHT / R
4. Release all controller buttons between each step.
5. When it says Controller Saved, tap the screen to play.

Note:
- Calibrated movement is deliberately digital, not analog.
- This is intentional for the 8BitDo Micro and other compact D-pad controllers where Safari may expose the D-pad as buttons, axes, or hat values.

Controls:
- iPhone touch: on-screen D-pad + STRAFE arrows + SHOOT / OPEN buttons
- Calibrated Bluetooth controller: whatever you taught the game with CAL
- Keyboard: WASD or arrow keys; Q/E strafe; Space to shoot; F/Z to open/use
- Debug: tap PAD on iPhone, or press G / ` on keyboard.
- Calibration on keyboard/desktop: press C.
