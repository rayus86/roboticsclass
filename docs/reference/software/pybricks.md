# PyBricks (EV3) Setup (MVP)

## Why PyBricks?
Real Python on EV3, direct motor/sensor APIs, smooth bridge from CodeHS.

## Quick Start
1. Open https://code.pybricks.com
2. Connect EV3 (ensure proper firmware)
3. Write simple program, download, run

## Sample
```python
from pybricks.hubs import EV3Brick
from pybricks.tools import wait

brick = EV3Brick()
for i in range(3):
    brick.speaker.beep()
    wait(400)
```

## Moving Local (Later)
Use VS Code for larger projects (multiple files, version control).

<!-- TEACHER NOTE:
Add local CLI workflow after initial hardware comfort.
-->