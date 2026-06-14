SeanFPS v0.8.1
===============

This is a one-line hotfix release for v0.8.

Fix:
- The zombie render callback now correctly receives the rel parameter:
  (x, yTop, yBot, dist, size, rel) => { ... }

Why:
- renderBillboard already passed rel as the sixth argument.
- The renderEnemies callback did not declare rel, so references to rel could throw ReferenceError in strict mode.

Everything else is unchanged from v0.8.

Controls:
- iPhone touch: on-screen D-pad + STRAFE arrows + SHOOT / OPEN buttons
- Bluetooth controller: D-pad or left stick to move/turn; A to shoot; B to open/use; shoulder buttons may strafe
- Keyboard: WASD or arrow keys; Q/E strafe; Space to shoot; F/Z to open/use
- Debug: press G or ` on a keyboard to show/hide controller debug.
