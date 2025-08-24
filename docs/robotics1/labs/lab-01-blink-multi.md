# Lab 1 (R1): Multi-Platform Blink / Beep

**Goal:** Observe timing & feedback on two platforms.

## Deliverables
- Notebook entry (Objective → Steps → Result → Reflection)
- Modified timing pattern
- Short comparison paragraph (EV3 vs Arduino if both attempted)

## Tasks
=== "EV3 (PyBricks)"
```python
from pybricks.hubs import EV3Brick
from pybricks.tools import wait

brick = EV3Brick()
pattern = [200, 800, 200, 800, 1200]
for d in pattern:
    brick.speaker.beep()
    wait(d)
```

Modify pattern to create a unique rhythm. Document why you chose it.

=== "Arduino"
```c++
int pattern[] = {200, 800, 200, 800, 1200};
void setup(){ pinMode(13, OUTPUT); }
void loop(){
  for(int i=0;i<5;i++){
    digitalWrite(13, HIGH); delay(pattern[i]);
    digitalWrite(13, LOW);  delay(150);
  }
  delay(1200);
}
```

Change pattern; add comments describing each segment.

## Reflection
1. Which platform gave clearer feedback and why?
2. How could you represent a more complex pattern (like Morse code)?

<!-- TEACHER NOTE:
If time short, assign second platform as optional extension.
-->