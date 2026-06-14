SeanFPS v0.5
=============

This ZIP contains v0.5 of the simple Doom/Wolfenstein-style iPhone browser game.

Files:
- index.html = the whole game in one file

Controls:
- iPhone touch: on-screen D-pad + STRAFE arrows + SHOOT / OPEN buttons
- Bluetooth controller: D-pad or left stick to move/turn; A to shoot; B to open/use; shoulder buttons may strafe
- Keyboard: WASD or arrow keys; Q/E strafe; Space to shoot; F/Z to open/use
- Restart: tap Restart, tap the screen after win/loss, or press R / Enter / Space

What changed from v0.4:
- Removed the final messageBody.innerHTML write from showIntro().
- The intro screen now restores from the static HTML content rather than writing HTML strings.
- Simplified the crosshair to a clean 3x3 white dot.
- Changed renderBillboard() so distance is a required parameter, not an ambiguous distOverride.
- Removed the per-frame controller-label update from render().
- Controller label updates are now event-driven, with a one-time poll fallback if iOS exposes the controller only after a button press.
- resetGame() now removes .down classes from SHOOT, OPEN, and STRAFE buttons as well as the D-pad.

Important iPhone note:
Do not open index.html directly from Files if you want the best chance of controller support.
Run it through Safari using a tiny local web server, or upload it as an HTML game to itch.io.

Local server command for a-Shell mini:
python3 -m http.server 8000

Then open Safari:
http://127.0.0.1:8000
