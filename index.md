# Introduction to Computer Science — Student Activity Guide

Welcome! Today you'll learn what computer science is and build your own projects using **Scratch**, a free block-coding platform. No experience needed — just curiosity!

**Website:** scratch.mit.edu (open in Safari on your iPad)

---

## Getting Started: Log In to Scratch

1. Open **Safari** on your iPad.
2. Go to **scratch.mit.edu**.
3. Tap **Sign In** (top right).
4. Enter the username and password your instructor gives you.
5. Tap **Create** (top menu) to start a new project.

You should see the Scratch editor with the orange cat on the stage.

> **iPad tip:** Turn your iPad **sideways** (landscape mode). The Scratch editor needs the wider view — portrait mode squishes the blocks and makes them hard to drag.

---

## The Scratch Editor — Know Your Way Around

```
┌──────────────────────────────────────────────────────────┐
│  Block Palette (left)  │  Code Area (center)  │  Stage  │
│                        │                      │ (top    │
│  Pick blocks from      │  Drag & snap blocks  │  right) │
│  these categories:     │  together here        │         │
│  • Motion              │                      │ Your    │
│  • Looks               │                      │ project │
│  • Sound               │                      │ runs    │
│  • Events              │                      │ here!   │
│  • Control             │                      │         │
│  • Sensing             │                      ├─────────┤
│  • Operators           │                      │ Sprite  │
│  • Variables           │                      │ List    │
│                        │                      │(bottom) │
└──────────────────────────────────────────────────────────┘
        ▲ Green Flag = Run     ▲ Stop Sign = Stop
```

**Important:** Each sprite has its own code. Tap a sprite in the sprite list to see and edit its code.

---

## Understanding the Stage: X/Y Coordinates and Layers

Before you start building, it helps to understand how Scratch knows **where** things are and **which sprite shows in front**.

### X/Y Coordinates — Where Sprites Live

The Scratch stage is a grid. Every spot on the stage has two numbers:

- **X** = left and right (horizontal)
- **Y** = up and down (vertical)

```
                    y: 180 (top)
                       ↑
                       |
  x: -240 (left) ─────┼───── x: 240 (right)
                       |
                       ↓
                    y: -180 (bottom)

              Center = x: 0, y: 0
```

| Direction | What changes | Example |
|---|---|---|
| Move **right** | x gets bigger (more positive) | x: 0 → x: 100 |
| Move **left** | x gets smaller (more negative) | x: 0 → x: -100 |
| Move **up** | y gets bigger (more positive) | y: 0 → y: 100 |
| Move **down** | y gets smaller (more negative) | y: 0 → y: -100 |

**Quick reference:**

| Position | Coordinates |
|---|---|
| Top-left corner | x: -240, y: 180 |
| Top-right corner | x: 240, y: 180 |
| Bottom-left corner | x: -240, y: -180 |
| Bottom-right corner | x: 240, y: -180 |
| Dead center | x: 0, y: 0 |

**Tip:** If you want to know the coordinates of any spot, drag your finger across the stage — the x and y values show at the bottom-right of the stage area.

### Layers — Which Sprite Shows in Front

When two sprites overlap, one shows in front of the other. This is called **layering** — think of it like stacking papers on a desk. The top paper covers the ones below it.

You can control layers with blocks in the **Looks** category:

| Block | What it does |
|---|---|
| `go to front layer` | Puts this sprite on top of all others |
| `go to back layer` | Puts this sprite behind all others |
| `go forward 1 layers` | Moves this sprite up one layer |
| `go backward 1 layers` | Moves this sprite back one layer |

**When you'll use this:**
- If a sprite's speech bubble is hidden behind another sprite, use `go to front layer` on that sprite.
- In a game, make sure your player sprite is in front of the background objects.
- Backdrops are always behind all sprites — you don't need layer blocks for those.

---

## Activity 1: Animate a Story (30 minutes)

### Your Goal

Create a short animated scene with at least 2 characters that do something when you press the green flag.

### Step-by-Step Instructions

#### Step 1: Choose a backdrop (2 min)

1. Look at the bottom-right corner of the screen — you'll see the stage thumbnail.
2. Tap the **backdrop icon** (the picture icon next to the sprite icon).
3. Tap **Choose a Backdrop** and pick one you like (try "Beach Malibu," "Castle," or "Space").

#### Step 2: Add your characters (3 min)

1. In the bottom-right **Sprite List**, tap the **cat face icon** with a "+" to add a sprite.
2. Tap **Choose a Sprite** and pick a character.
3. Add at least **one more sprite** (you need 2 total).
4. (Optional) To delete the default cat: tap the cat sprite, then tap the trash can icon on it.

#### Step 3: Make your first sprite do something (5 min)

1. Tap your **first sprite** in the sprite list to select it.
2. Go to the **Events** category (yellow) in the block palette.
3. Drag `when green flag clicked` into the code area.
4. Go to the **Looks** category (purple).
5. Drag `say [Hello!] for [2] seconds` and snap it below the green flag block.
6. Change the text inside the say block to whatever you want your character to say.
7. Press the **green flag** above the stage to test it!

#### Step 4: Add motion (5 min)

1. With the same sprite selected, go to **Motion** (blue).
2. Drag `glide [1] secs to x: [___] y: [___]` and snap it below your say block.
3. Change the x and y numbers to move your sprite to a different spot. (See the **X/Y Coordinates** section above for how the grid works.)
4. Press the green flag to see your sprite talk and then glide!

#### Step 5: Make your second sprite do something (5 min)

1. Tap your **second sprite** in the sprite list.
2. Add a `when green flag clicked` block (Events).
3. Add blocks to make this sprite do something different:
   - **Ideas:** `say` something, `glide` to a spot, `change size by [20]`, `switch costume to` a different look
4. Press the green flag — both sprites should do their thing at the same time!

#### Step 6: Add timing with wait blocks (5 min)

To make sprites "talk" to each other, use the **wait** block:

**Sprite 1 code:**
```
when green flag clicked
say [Hey, have you seen the treasure?] for (3) seconds
```

**Sprite 2 code:**
```
when green flag clicked
wait (3) seconds
say [It's hidden behind the castle!] for (3) seconds
```

The `wait` block on Sprite 2 makes it pause while Sprite 1 is talking.

#### Step 7: Add sound (3 min)

1. Select a sprite.
2. Go to the **Sound** category (pink).
3. Drag `play sound [___] until done` into your code stack.
4. To add new sounds: tap the **Sounds** tab at the top, then **Choose a Sound**.

#### Step 8: Test and polish (2 min)

1. Press the green flag and watch your whole animation.
2. Adjust timing, position, or dialogue until you're happy with it.

### Bonus Challenges (if you finish early)

- Add a **third sprite** that enters the scene late (use a long `wait` block).
- Make a sprite **change costumes** in a loop to create animation (Looks → `next costume` inside a `repeat` block).
- Add a **second backdrop** and switch to it partway through (Looks → `switch backdrop to`).

---

## Activity 2: Build a Game — "Catch the Stars" (35 minutes)

### Your Goal

Build a game where you move a character to catch falling objects and earn points.

### Step-by-Step Instructions

#### Step 1: Set the scene (3 min)

> **Don't worry!** Your Activity 1 project is saved automatically to your Scratch account. Starting a new project won't delete it — you can find it later at scratch.mit.edu/mystuff.

1. Start a **new project** (File → New).
2. Choose a fun backdrop (try "Blue Sky," "Stars," or "Colorful City").
3. Keep the cat as your catcher, or pick a different sprite (bowl, basket, character, etc.).
4. Make your catcher sprite **small** — go to the sprite info and set size to about 60.

#### Step 2: Make the catcher follow your finger (5 min)

1. Select your **catcher sprite**.
2. Build this code:

```
when green flag clicked
forever
    go to x: (mouse x) y: (-150)
```

**How to build it:**
1. Events → drag `when green flag clicked`
2. Control → drag `forever` and snap it below
3. Motion → drag `go to x: [___] y: [___]` inside the forever loop
4. Sensing → drag `mouse x` into the x slot (replace the number). On iPad, "mouse x" really means **your finger position** — it tracks where you last touched the screen.
5. Type `-150` in the y slot (this keeps the catcher at the bottom)

**Test it!** Press the green flag and drag your finger across the screen. The catcher should follow left and right along the bottom.

#### Step 3: Create a falling object (5 min)

1. Add a **new sprite** — pick a star, apple, donut, or whatever you want to catch.
2. Make it small (size: 50 or so).
3. Select the falling object sprite and build this code:

```
when green flag clicked
forever
    go to x: (pick random (-200) to (200)) y: (180)
    glide (2) secs to x: (x position) y: (-180)
```

**How to build it:**
1. Events → `when green flag clicked`
2. Control → `forever`
3. Motion → `go to x: [___] y: [___]`
   - Operators → drag `pick random [1] to [10]` into the x slot, change to `-200` and `200`
   - Type `180` in the y slot
4. Motion → `glide [1] secs to x: [___] y: [___]`
   - Change `1` to `2`
   - Motion → drag `x position` into the glide x slot
   - Type `-180` in the glide y slot

**Test it!** The star should appear at a random spot at the top, then slowly fall down, then repeat.

#### Step 4: Create a score variable (2 min)

1. Go to the **Variables** category (dark orange).
2. Tap **Make a Variable**.
3. Name it `score` and tap OK.
4. You'll see the score display appear on the stage.

#### Step 5: Detect when you catch the star (5 min)

Still on the **falling object** sprite, add this inside the `forever` loop, **after** the `glide` block:

```
when green flag clicked
set [score] to (0)
forever
    go to x: (pick random (-200) to (200)) y: (180)
    glide (2) secs to x: (x position) y: (-180)
    if <touching [catcher sprite name]?> then
        change [score] by (1)
    end
```

**How to build the detection part:**
1. Variables → drag `set [score] to [0]` right below the green flag (before forever)
2. Control → drag `if <> then` inside the forever loop, after the glide block
3. Sensing → drag `touching [___]?` into the diamond-shaped slot
4. In the dropdown, select your catcher sprite's name
5. Variables → drag `change [score] by [1]` inside the if block

**Test it!** Catch the falling star with your catcher. The score should go up by 1 each time!

#### Step 6: Make missed objects reset (3 min)

Right now, if you miss the star, it just glides off screen and teleports back. Let's make that cleaner. Your full falling object code should look like:

```
when green flag clicked
set [score] to (0)
forever
    go to x: (pick random (-200) to (200)) y: (180)
    glide (2) secs to x: (x position) y: (-180)
    if <touching [catcher sprite name]?> then
        change [score] by (1)
        play sound [pop] until done
    end
```

The `forever` loop already handles the reset — after the glide and the if-check, it loops back to the top and picks a new random x position.

#### Step 7: Customize your game! (12 min)

Now make it YOUR game. Pick any of these upgrades:

| Upgrade | How to do it |
|---|---|
| **Add a sound on catch** | Inside the `if touching` block, add: Sound → `play sound [pop] until done` |
| **Make it speed up** | Create a `speed` variable. Set it to `2` at start. Use `speed` in the glide time. Add `change speed by (-0.1)` inside the if block so it gets faster. |
| **Add more falling objects** | Long-press the falling sprite in the sprite list → tap **Duplicate**. The code copies automatically! Change the costume to a different object. |
| **Add a "bad" object** | Duplicate the falling sprite, change its costume to something bad (bomb, ghost). In its code, change `change score by 1` to `change score by -1`. |
| **Add a start screen** | Make a sprite that says "Tap to Start!" and use `when this sprite clicked` → `broadcast [start]`. Change all `when green flag clicked` to `when I receive [start]`. |
| **Add lives** | Create a `lives` variable, set to 3. If the star reaches the bottom without being caught, `change lives by -1`. If `lives = 0`, `stop all`. |

---

## Pair Testing & Debugging (10 minutes)

### Instructions

1. **Trade iPads** with the person next to you.
2. **Play their game** for 3 minutes. Try to break it! (That's what testers do.)
3. **Write down** (or remember):
   - One thing that works really well
   - One bug or weird behavior you found
4. **Give your iPad back** and tell your partner what you found.
5. **Fix one bug** your partner found (5 minutes).

### Common Bugs and How to Fix Them

| Bug | Likely cause | Fix |
|---|---|---|
| Nothing happens when I press green flag | Missing `when green flag clicked` on top | Add the event block at the top of each code stack |
| Sprite shoots off screen | `move` block without a loop or edge check | Add `if on edge, bounce` inside the loop |
| Score doesn't reset when restarting | Missing `set score to 0` at the start | Add `set [score] to (0)` right after `when green flag clicked` |
| Two sprites do the same thing | Edited the wrong sprite's code | Click each sprite and check its code separately |
| Falling object freezes mid-fall | Another block is waiting/blocking | Check for `wait` blocks or `play sound until done` that might stall |
| Catcher follows finger but is invisible | Sprite is too small or hidden | Check size (increase it) or add a `show` block at start |

---

## Activity 3: Creative Remix Challenge (20 minutes)

### Choose Your Path

**Option A — Level Up Your Game**
Take your "Catch the Stars" game and add a big new feature from the upgrade table above.

**Option B — Build Something New**
Start a brand-new project. Here are some ideas:

| Idea | Key blocks you'll need |
|---|---|
| **Quiz game** | `ask [question] and wait` + `if <answer = [correct]>` |
| **Music maker** | Multiple sprites, each plays a different sound `when this sprite clicked` (expand on the beat maker demo!) |
| **Generative art** | Pen extension + `repeat` + `turn` + `change pen color`. Try different turn angles! |
| **Virtual pet** | Variables for hunger, happiness. Buttons to feed/play. `change hunger by -1` over time. |
| **Animated greeting card** | Costume switching, backdrop changes, sound, glide animations |
| **Maze game** | `if <touching color [wall]?> then [go to start position]` |

**Option C — Explore and Learn**
1. Go to **scratch.mit.edu/explore/projects/all**.
2. Find a project you think is cool.
3. Tap **See Inside** to look at the code.
4. Try to figure out how one feature works.
5. Explain it to the person next to you.

**Option D — Remix a Demo**
Open the generative art or beat maker project your instructor shared with the class. Tap **See Inside**, then **Remix**. Some ideas:
- **Art remix:** Change the turn angle (try 91, 121, or 144), change the pen size, add a second spiral with a different starting position.
- **Music remix:** Add more drum pads with new sounds, change the colors, add a `forever` loop with `wait` blocks to create an auto-playing beat.

---

## What's Next? Keep Coding!

Your Scratch projects are saved to your account. Here's how to keep going:

| Resource | Link | What it is |
|---|---|---|
| **Scratch** | scratch.mit.edu | Keep building! Try the tutorials at scratch.mit.edu/ideas |
| **Code.org** | code.org | Free CS courses — works on iPad |
| **Replit** | replit.com | Write real Python code in your browser — free, works on iPad |
| **Khan Academy** | khanacademy.org/computing | Learn JavaScript with interactive lessons |

Computer science is used in **every field** — music, art, medicine, sports, gaming, fashion, filmmaking, space exploration. Whatever you're into, CS can be part of it.
