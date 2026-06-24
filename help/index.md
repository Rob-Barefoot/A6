# Scratch Cheat Sheet

**Website:** scratch.mit.edu | **Works on:** iPad (Safari), Chromebook, laptop, desktop

> **iPad users:** Turn your iPad to **landscape** (sideways) mode for the best experience. When dragging blocks, use a **press-and-hold then drag** motion.

---

## The Scratch Editor

| Area | Where | What it does |
|---|---|---|
| **Stage** | Top right | Shows your running project |
| **Sprite list** | Bottom right | Your characters and objects |
| **Block palette** | Left side | Blocks you can drag into your code |
| **Code area** | Center | Snap blocks together here |
| **Green flag** | Above the stage | Runs your project |
| **Stop sign** | Above the stage | Stops your project |

---

## Block Categories

### Events (yellow) — Start things

| Block | What it does |
|---|---|
| `when green flag clicked` | Runs code when you press the green flag |
| `when this sprite clicked` | Runs code when you tap/click a sprite |
| `when space key pressed` | Runs code when you press a key *(on iPad, opens the on-screen keyboard)* |

### Motion (blue) — Move sprites

| Block | What it does |
|---|---|
| `move 10 steps` | Moves the sprite forward |
| `turn 15 degrees` | Rotates the sprite |
| `go to x: 0 y: 0` | Jumps to a specific spot |
| `glide 1 secs to x: 0 y: 0` | Slides smoothly to a spot |
| `if on edge, bounce` | Bounces off the edge of the stage |

### Looks (purple) — Change appearance

| Block | What it does |
|---|---|
| `say Hello! for 2 seconds` | Shows a speech bubble |
| `think Hmm... for 2 seconds` | Shows a thought bubble |
| `switch costume to` | Changes the sprite's picture |
| `change size by 10` | Makes the sprite bigger or smaller |
| `hide` / `show` | Makes the sprite invisible or visible |
| `go to front layer` | Puts this sprite in front of all others |
| `go backward 1 layers` | Moves this sprite back one layer |

### Sound (pink) — Play sounds

| Block | What it does |
|---|---|
| `play sound meow until done` | Plays a sound and waits |
| `start sound meow` | Plays a sound without waiting |

### Control (orange) — Loops & decisions

| Block | What it does |
|---|---|
| `wait 1 seconds` | Pauses before the next block |
| `repeat 10` | Runs blocks inside it 10 times |
| `forever` | Runs blocks inside it nonstop |
| `if <> then` | Runs blocks only if something is true |
| `if <> then / else` | Does one thing if true, another if false |

### Sensing (light blue) — Detect things

| Block | What it does |
|---|---|
| `touching mouse-pointer?` | True if sprite touches the cursor/finger |
| `touching color?` | True if sprite touches a specific color |
| `touching Sprite2?` | True if sprite touches another sprite |
| `mouse x` / `mouse y` | The current finger/cursor position (on iPad, tracks your last touch) |
| `key space pressed?` | True if a key is being pressed *(on iPad, opens the on-screen keyboard)* |

### Operators (green) — Math & logic

| Block | What it does |
|---|---|
| `pick random 1 to 10` | A random number in that range |
| `+ - * /` | Math operations |
| `< > =` | Comparison (less than, greater than, equal) |
| `and` / `or` / `not` | Combine true/false conditions |

### Variables (dark orange) — Store data

| Block | What it does |
|---|---|
| `set score to 0` | Sets a variable to a value |
| `change score by 1` | Adds to a variable |

---

## Common Patterns

### Make a sprite follow your finger (iPad)

```
when green flag clicked
forever
  go to x: (mouse x) y: (mouse y)
```

### Make a sprite bounce around

```
when green flag clicked
point in direction (pick random 0 to 360)
forever
  move 5 steps
  if on edge, bounce
```

### Make sprites "talk" to each other

```
Sprite 1:                        Sprite 2:
when green flag clicked          when green flag clicked
say "Hi!" for 2 seconds          wait 2 seconds
                                 say "Hello!" for 2 seconds
```

### Simple score counter

```
when green flag clicked
set score to 0
forever
  if <touching Sprite2?> then
    change score by 1
    wait 0.5 seconds
```

---

## Tips

- **Each sprite has its own code.** Click a sprite to see and edit its code.
- **Right-click a sprite** to duplicate it (copies the code too!).
- **Use "See Inside"** on any project in the Scratch community to learn how it was made.
- **Save often!** Scratch auto-saves when you're signed in.
- **Undo:** Press Ctrl+Z (or Cmd+Z on Mac) to undo.
