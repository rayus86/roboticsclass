# Lesson 1 (R1): Introduction & Platforms Overview

**Duration:** ~50 min  
**Objectives:**
- Define a robot (sense–process–act).
- Compare three platforms (EV3, Arduino, Drone) at a high level.
- Run a first simple program (beep or blink).

## Warm-Up
List two systems you think are robots and one you think is not. Be ready to justify.

## Mini-Lecture Topics
- What makes a robot?
- Domains: industrial, medical, aerial, consumer, competition
- Platform overview (EV3 vs Arduino vs Drone)

## First Program (PyBricks EV3)
```python
from pybricks.hubs import EV3Brick
from pybricks.tools import wait

brick = EV3Brick()
for i in range(3):
    brick.speaker.beep()
    wait(400)
```

## Alternate (Arduino Blink)
```c++
void setup(){ pinMode(13, OUTPUT); }
void loop(){
  digitalWrite(13, HIGH); delay(500);
  digitalWrite(13, LOW);  delay(500);
}
```

## Reflection Prompt
What part of programming this felt familiar or unfamiliar compared to any past coding experience?

<!-- TEACHER NOTE:
Next lesson: deeper platform comparison & classification activity.
-->