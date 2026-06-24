# Introduction to Computer Science with Block Coding

## Instructor Lesson Plan — 3-Hour Training Session

| Detail | Value |
|---|---|
| **Audience** | Teenagers, ages 12–18 |
| **Group size** | ~20 learners |
| **Duration** | ~3 hours 30 minutes (210 minutes) |
| **Platform** | Scratch (https://scratch.mit.edu) |
| **Device** | iPad with Safari (internet required) |
| **Prerequisites** | None — no prior coding experience needed |

---

## Before the Session

### Instructor prep (do these at least 1 day before)

1. **Create a Scratch teacher account** at https://scratch.mit.edu/educators — this lets you create a class and student accounts in bulk so learners don't need email addresses.
2. **Create a Scratch class** and generate 20+ student usernames/passwords. Print or prepare a shared slide with login credentials.
3. **Test Scratch on an iPad in Safari** — confirm the block editor loads and drag-and-drop works. Scratch works well on iPads running iOS 15+ with Safari.
4. **Prepare starter projects** (optional but recommended):
   - Upload a "Starter Sprites" project with 3–4 fun sprites and a backdrop that learners can remix in Activity 2.
   - Share the project link with the class.
5. **Print or prepare a "Scratch Cheat Sheet"** with key block categories (Motion, Looks, Events, Control, Sensing, Operators, Variables) — one per learner or pair.
6. **Ensure Wi-Fi can handle 20+ simultaneous connections** to scratch.mit.edu.
7. **Have a backup plan**: Download the Scratch app from the App Store in case Wi-Fi is spotty. Projects save locally in the app.
8. **Pre-build the two live demo projects** (generative art spiral + beat maker drum machine). Test them on your iPad. Save finished versions to the class account so you have a backup if the live build doesn't go smoothly, and so learners can remix them during Activity 3.

### Room setup

- Arrange tables in clusters of 4 so pairs can collaborate and share screens.
- Project your iPad or laptop screen for live demos.
- Have a whiteboard or flip chart for CS concept brainstorming.
- **Set all iPads to landscape (sideways) orientation** before learners arrive. Scratch is nearly unusable in portrait mode — the block palette, code area, and stage compete for space.

---

## Session at a Glance

| Time | Block | Duration | Type |
|---|---|---|---|
| 0:00–0:15 | Welcome & Icebreaker | 15 min | Discussion |
| 0:15–0:30 | What Is Computer Science? | 15 min | Interactive lecture |
| 0:30–0:50 | Scratch Tour & First Steps | 20 min | Guided hands-on |
| 0:50–1:05 | Activity 1, Part A: Guided Setup | 15 min | Guided hands-on |
| 1:05–1:10 | Activity 1: Check-in | 5 min | Discussion |
| 1:10–1:25 | Activity 1, Part B: Independent Build | 15 min | Hands-on |
| 1:25–1:35 | **Break** | 10 min | — |
| 1:35–1:50 | Think Like a Programmer | 15 min | Interactive lecture |
| 1:50–2:15 | Activity 2, Part A: Guided Build | 25 min | Guided hands-on |
| 2:15–2:20 | Activity 2: Check-in | 5 min | Discussion |
| 2:20–2:35 | Activity 2, Part B: Customize & Extend | 15 min | Hands-on |
| 2:35–2:45 | Pair Testing & Debugging | 10 min | Collaborative |
| 2:45–3:00 | "One More Thing" — Live Demos | 15 min | Instructor demo |
| 3:00–3:20 | Activity 3: Creative Remix Challenge | 20 min | Open-ended hands-on |
| 3:20–3:30 | Showcase & Wrap-Up | 10 min | Presentations / discussion |

---

## Detailed Session Plan

---

### Block 1: Welcome & Foundations (0:00–0:50)

#### Welcome & Icebreaker (15 min)

**Goal:** Build energy, learn names, and prime learners to think computationally.

1. **Introduce yourself** (2 min) — Keep it short. Share one fun fact about how you got interested in tech.
   - **Instructor note:** Teens warm up faster if you're relatable. If you have a story about being a beginner or making a funny mistake, use it. Avoid corporate-speak. "I once accidentally deleted my entire project 10 minutes before a deadline" lands better than "I've been in the industry for 15 years."

2. **Icebreaker: "The Human Robot"** (13 min)
   - Ask for a volunteer to be the "robot." They can only follow exact instructions.
   - The rest of the group must give step-by-step instructions to get the robot to walk across the room and pick up an object (like a marker on a table).
   - Rules: The robot interprets everything literally — no common sense, no assumptions.

   **Common commands and how they backfire:**

   | What they say | What the robot does | Why it fails |
   |---|---|---|
   | "Walk forward" | Walks forward and never stops — walks into a wall or off the stage | No stop condition. They needed: "Take 5 steps forward" or "Walk forward until you reach the table." |
   | "Pick it up" | Stands still, confused. What is "it"? | Undefined reference. They needed: "Pick up the red marker on the table." |
   | "Go to the table" | Walks directly in a straight line, crashes into chairs in the way | No obstacle awareness. They needed: "Turn left. Walk 3 steps. Turn right. Walk 6 steps." |
   | "Grab the marker" | Slaps hand down on the marker without wrapping fingers around it | "Grab" isn't precise enough. They needed: "Open your hand. Lower it around the marker. Close your fingers. Lift your hand." |
   | "Turn around" | Spins in a full 360° circle and faces the same direction | Ambiguous. They needed: "Turn 180 degrees" or "Turn to face the back wall." |
   | "Walk to the marker and pick it up" | Does both simultaneously — walks while swiping at the air | Two commands at once with no sequence. They needed to separate: first walk, then stop, then pick up. |
   | "Move right" | Slides sideways without turning (like a crab) | They probably meant "Turn right, then walk forward" — but the robot followed literally. |
   | "Go faster" | Robot has no concept of speed levels — stands still, confused | No baseline defined. They needed: "Take 2 steps every second" instead of "1 step every second." |

   **Tips for running the activity:**
   - Coach the robot volunteer beforehand: "Your job is to be as literal as possible. If the instruction is ambiguous, do the funniest wrong interpretation."
   - Let the group fail a few times before intervening — the laughs from mistakes make the lesson stick.
   - If the group gets stuck, prompt them: "What is the FIRST small thing the robot needs to do?" This teaches decomposition.
   - For a large group, have 2–3 "rounds" with different volunteers as the robot so more people participate.
   - If short on time, simplify the task: just walk to a spot and stop (skip picking up the object).

   **Debrief** (3 min): Ask the group:
   - *What was hard about giving instructions?*
   - *What happened when instructions were vague?*
   - *How did you fix a command that went wrong?* (This is debugging!)
   - *What's the smallest step you had to break things down to?*

   **Key takeaway**: Computers follow instructions exactly — programming is about writing clear, precise instructions. When something goes wrong, it's almost always because the instructions weren't specific enough, not because the computer is broken. That's what debugging is: finding and fixing the unclear instruction.

#### What Is Computer Science? (15 min)

**Goal:** Demystify CS and connect it to things teens already use.

1. **Quick poll** (3 min): "Raise your hand if you've used any of these today..." (phone, social media, games, maps, music streaming). Point out: every one of those runs on code.
   - **Instructor note:** This works best if you move fast and keep it energetic. Rattle off examples: "Snapchat? Code. TikTok algorithm? Code. Your Spotify Discover Weekly? An algorithm wrote that playlist for you." The goal is to make CS feel relevant, not academic.

2. **CS is more than coding** (7 min) — Briefly cover with examples they can relate to:
   - **Algorithms**: A playlist's shuffle is an algorithm. A recipe is an algorithm.
   - **Decomposition**: Breaking a big task into small steps (like the robot activity).
   - **Pattern recognition**: Instagram filters recognize faces using patterns.
   - **Abstraction**: You don't need to understand how Wi-Fi works to use it — that's abstraction.

3. **Why block coding?** (5 min)
   - Show a quick side-by-side of a Scratch block stack vs. the same logic in Python text code.
   - Point: Blocks and text code express the *same ideas*. Blocks let you focus on logic without worrying about typos and syntax.
   - Name-drop professionals who started with Scratch or block coding.

#### Scratch Tour & First Steps (20 min)

**Goal:** Every learner logs in, navigates the editor, and makes a sprite move.

1. **Log in** (5 min)
   - Display the class login credentials.
   - Have learners open Safari → scratch.mit.edu → Sign In.
   - Click "Create" to open a new project.
   - **Fallback if a learner can't sign in:** They can use Scratch without an account — they just can't save to the cloud. On iPad, the backup is the **Scratch app** (free in the App Store), which saves projects locally. Have 2–3 iPads with the app pre-installed as spares.
   - **Tell learners:** "Open your Student Activity Guide and follow the Getting Started section."

2. **Live demo: Editor tour** (10 min) — Walk through on your projected screen:
   - **Stage** (top right): Where your project runs.
   - **Sprite list** (bottom right): Your characters and objects.
   - **Block palette** (left): Drag blocks from here.
   - **Code area** (center): Snap blocks together here.
   - **Green flag / Stop sign**: Run and stop your project.
   - Demo dragging a few blocks:
     - `when green flag clicked` → `move 10 steps` → Click green flag. The cat moves!
     - Add `turn 15 degrees` → Click green flag. Now it moves and turns.
     - Wrap in `forever` loop. The cat spins continuously.

3. **Try it yourself** (5 min)
   - Challenge: "Make the Scratch cat do something — anything. Move, spin, change color, say something. You have 5 minutes. Go!"
   - Walk the room and help anyone who's stuck.
   - **Instructor note:** This unstructured time is critical. It gives learners permission to poke around without fear of doing it wrong. If someone says "I don't know what to do," say: "Try dragging any block into the code area and pressing the green flag. See what happens." Avoid giving a specific task here — the point is exploration and building confidence that nothing will break.

---

### Activity 1: Animate a Story (0:50–1:25) — 35 min

**Goal:** Learners create a short animated scene using motion, looks, sound, and events blocks.

**Concepts covered:** Sequencing, events, parallelism (multiple sprites acting at once).

**Tell learners:** "Open your Student Activity Guide to Activity 1. Follow the step-by-step instructions there — I'll demo each step on the projector first."

#### Part A: Guided Setup (0:50–1:05) — 15 min

Present the challenge, then walk learners through the setup live on the projector while they follow along.

> **Your challenge:** Create a short animated scene with at least 2 characters. It should have:
> - A backdrop (go to the backdrop library and pick one)
> - At least 2 sprites (characters or objects)
> - Each sprite does something when the green flag is clicked
> - At least one sprite "says" or "thinks" something
> - Bonus: Add a sound effect or music

**Guided scaffolding (do this live as they follow along):**

1. **(5 min)** Show how to:
   - Change the backdrop (tap the backdrop icon, choose from library)
   - Add a new sprite (tap the sprite icon, choose from library)
   - Delete the default cat if they want (tap the sprite, then tap the trash icon)
   - **iPad tip for the group:** "If you accidentally zoom in, pinch with two fingers to zoom back out. And when dragging blocks, press and hold for a moment before you drag."

2. **(5 min)** Show useful blocks:
   - **Looks**: `say [Hello!] for 2 seconds`, `switch costume to`, `change size by`
   - **Motion**: `glide 1 secs to x: y:`, `go to x: y:`
   - **Sound**: `play sound [meow] until done`
   - **Events**: `when green flag clicked`
   - Quick reminder: "Check the X/Y Coordinates section in your activity guide if you're not sure what the x and y numbers mean."

3. **(5 min)** Walk the room while learners set up their backdrop and sprites. Make sure everyone has:
   - A backdrop selected
   - At least 2 sprites added
   - A `when green flag clicked` block on at least one sprite

#### Check-in (1:05–1:10) — 5 min

Pause the room. This is your chance to catch problems before they snowball.

1. **Quick pulse:** "Raise your hand if you have at least 2 sprites and a backdrop." (If more than a few hands are down, demo the setup one more time.)
2. **Address the #1 issue you're seeing.** Common ones:
   - "I see some of you adding blocks but nothing happens when you press the green flag — make sure every code stack starts with a yellow event block on top."
   - "Remember, each sprite has its own code. Tap a sprite in the sprite list at the bottom to switch to its code."
3. **Show one trick** based on what you're seeing: the `wait` block for timing, or `glide` for smooth motion.

#### Part B: Independent Build (1:10–1:25) — 15 min

Let them build freely. Your main job now is walking the room.

1. **(12 min)** Build time. Common help requests:
   - "My sprite isn't doing anything" → Check if they have a `when green flag clicked` block on top.
   - "Both sprites do the same thing" → Each sprite has its own code area. Tap a sprite to see/edit its code.
   - "How do I make them talk to each other?" → Show the `wait` block to create timing/pauses between dialogue.
   - "My sprite is behind the other one" → Show the `go to front layer` block (Looks category). Reference the Layers section in the activity guide.

2. **(3 min)** Quick share: Ask 2–3 volunteers to show their animation to the group. Celebrate creativity — keep feedback specific: "I love how you used the wait block to make them take turns talking."

**Instructor notes:**
- Resist the urge to over-prescribe. Let learners experiment.
- If someone finishes early, challenge them to add: a third sprite, a costume animation (switching costumes in a loop), or a second scene.
- **Watch for the "silent stuck" learner** — the one who isn't asking for help but also isn't making progress. Walk by their screen and ask "What are you trying to make happen?" rather than "Do you need help?" The first question is less embarrassing.
- **Pairing strategy:** If you notice a learner who's far ahead sitting near one who's struggling, casually say "Hey [advanced learner], [other learner] is working on something cool — can you two compare ideas?" This creates organic peer help without singling anyone out.

---

### Break (1:25–1:35) — 10 min

Encourage learners to step away from screens. Good time to grab water, stretch.

**Instructor note:** Use the break to:
- Scan the room for any learner who seems checked out or frustrated — approach them casually when the break ends and offer 1-on-1 help.
- Check in on Wi-Fi performance. If things are lagging, this is a good time to close unnecessary tabs on your demo machine.
- Preview Activity 2 on your own device so you can demo it smoothly.
- If you noticed common mistakes in Activity 1 (e.g., most students forgot the `when green flag clicked` block), plan a 30-second callout after the break: "Quick tip before we start — remember, every code stack needs an event block on top!"

**Transition note:** When the break ends, tell the group: "We're starting a brand-new project for Activity 2. Tap File → New. **Don't worry — your Activity 1 project is saved automatically.** You can find it anytime at scratch.mit.edu/mystuff."

---

### Block 2: Think Like a Programmer (1:35–2:35)

#### Think Like a Programmer (1:35–1:50) — 15 min

**Goal:** Introduce loops, conditionals, and variables — the building blocks of every program.

1. **Loops** (5 min)
   - Real-world example: "Brush teeth → rinse → repeat" — that's a loop.
   - Show `repeat 10` and `forever` blocks in Scratch.
   - Demo: Make a sprite walk across the screen using `repeat 100 [move 2 steps]` vs. `move 200 steps` — loops give you smooth animation.

2. **Conditionals (if/else)** (5 min)
   - Real-world example: "If it's raining, bring an umbrella. Else, wear sunglasses."
   - Show `if <> then` and `if <> then / else` blocks.
   - Demo: `if <touching edge?> then [turn 180 degrees]` — the sprite bounces off walls.

3. **Variables** (5 min)
   - Real-world example: A scoreboard at a game — the score is a variable that changes.
   - Show how to create a variable in Scratch (tap "Make a Variable").
   - Demo: Create a `score` variable, use `change score by 1` to increment it.

#### Activity 2: Build a Game (1:50–2:35) — 45 min

**Goal:** Each learner builds a playable game using loops, conditionals, and variables.

**Game option: "Catch the Stars"** (recommended — simple, fun, teaches core concepts)

**Tell learners:** "Open your Student Activity Guide to Activity 2. We'll build this game step by step — I'll demo each step on the projector, then you follow along on your iPad."

> **Your challenge:** Build a game where a character catches falling objects to earn points.

##### Part A: Guided Build — Steps 1–5 (1:50–2:15) — 25 min

Demo each step on the projector. Give learners time to follow along before moving to the next step.

| Step | Time | What to do |
|---|---|---|
| 1. Set the scene | 3 min | Choose a backdrop. Keep or change the main sprite (the "catcher"). Remind learners: "Your Activity 1 project is saved — this is a new project." |
| 2. Control the catcher | 5 min | Make the catcher follow your finger: `forever [go to x: (mouse x) y: -150]`. Tell learners: "The block says 'mouse x' but on iPad it tracks your finger position." |
| 3. Add a falling object | 5 min | Add a second sprite (a star, apple, etc.). Code it to start at a random position at the top: `when green flag clicked → forever [go to x: (pick random -200 to 200) y: 180 → glide 2 secs to x: (x position) y: -180]`. |
| 4. Create a score variable | 2 min | Tap Variables → Make a Variable → name it `score`. Add `set score to 0` after the green flag on the falling sprite. |
| 5. Detect catching | 10 min | On the falling sprite, inside the `forever` loop after the `glide`: `if <touching [catcher]?> then [change score by 1]`. **This is the hardest step — demo it slowly.** Show exactly where the `if` block goes (inside `forever`, after `glide`), how to find `touching` in Sensing, and how to select the catcher sprite from the dropdown. Walk the room and help individually. |

**Instructor notes for Part A:**
- Walk the room constantly. iPad touch targets are small — help learners who struggle with dragging blocks into tight spots.
- **Step 5 is the crux.** Expect to spend extra time here. The nesting (`if` inside `forever`) and the dropdown selection trip up most beginners. Demo this on the projector, then walk to each table and check.
- **The `mouse x` / `mouse y` name:** On iPad, "mouse" position actually tracks the last touch point. This works perfectly for finger-following sprites, but learners may be confused by the name — just say "this tells the sprite where your finger is."
- **Don't panic if it's messy.** Teens' code will have blocks scattered everywhere. That's fine — it means they're experimenting. Only intervene if they're genuinely stuck.

##### Check-in (2:15–2:20) — 5 min

Pause the room. Everyone stops and tests.

1. **"Everyone press the green flag."** Walk the room quickly.
2. **Quick diagnostic:** "Raise your hand if your score goes up when you catch the star." Celebrate those who got it working.
3. **For those who didn't get it working:** Troubleshoot the top issues live on the projector:
   - Score doesn't change → The `if <touching?>` block might be outside the `forever` loop, or the wrong sprite is selected in the dropdown.
   - Star doesn't fall → Check that the falling sprite (not the catcher) has the glide code.
   - Catcher doesn't move → Missing `forever` loop around the `go to x: (mouse x)` block.
4. **Checkpoint rescue:** If a learner is more than one step behind, help them catch up now, or offer: "I have a working version saved — you can remix it and jump straight to customizing." (Pre-save a checkpoint project to the class account so you can share the link.)

##### Part B: Customize & Extend (2:20–2:35) — 15 min

Now it's their game. Let them make it unique.

> **Pick any upgrades from your Student Activity Guide, or invent your own:**
> - Add a sound effect when you catch the star
> - Make the star fall faster over time (create a `speed` variable)
> - Duplicate the falling sprite to add more objects
> - Add a "bad" object that costs points
> - Add a start screen or game-over screen
> - Add a `lives` variable — subtract 1 when you miss

**Instructor notes for Part B:**
- This is creative exploration time. Walk around, encourage, help unblock.
- If a learner is ahead, challenge them to: add increasing difficulty, add a timer, or add multiple falling objects with different point values.
- If a learner is behind, pair them with a neighbor. Getting *something* customized (even just a sound effect) gives them ownership of the project.
- **Duplicate sprites on iPad:** Learners need to **long-press** the sprite in the sprite list → tap **Duplicate**. There's no right-click on iPad. Call this out to the group.

#### Pair Testing & Debugging (2:35–2:45) — 10 min

**Goal:** Teach debugging through peer testing.

1. **Swap iPads** with a neighbor (or share links via the class page).
2. **Play your partner's game** for 3 minutes.
3. **Give feedback**: Tell your partner:
   - One thing that works well
   - One bug or weird behavior you found
4. **Fix one bug** your partner found (4 min).

**Debrief** (2 min): Ask the group:
- *Did anyone find a bug they didn't expect?*
- *How did you fix it?*
- **Key takeaway**: Professional developers spend more time debugging than writing new code. Testing is a superpower.

---

### "One More Thing" — Live Demos (2:45–3:00) — 15 min

**Goal:** Blow the doors off what learners think is possible with block coding. These two demos are fast, visual, and designed to re-energize the room before the final creative block.

**Instructor note:** These are *your* demos — learners watch, react, and ask questions. They don't build along. This is the "mic drop" moment of the session.

#### Demo 1: Generative Art with the Pen Extension (7 min)

**What they'll see:** A spiral of colorful shapes drawn in real time — generative art from ~12 blocks.

**Setup (30 sec):**
1. Open a new Scratch project on your projected screen.
2. Tap the **Add Extension** button (bottom-left, the blocks-with-a-plus icon).
3. Select **Pen**. The green Pen blocks appear in your palette.
4. Hide the cat sprite (Looks → `hide`) so the drawing is clean.

**Build live (4 min) — talk as you drag each block:**

Say: "We've been building games and animations. But code can also make *art*. Watch this."

```
when green flag clicked
erase all
pen up
go to x: (0) y: (0)
set pen size to (2)
pen down
repeat (200)
    move (1) steps
    turn right (61) degrees
    change pen color by (1)
    change [steps] by (0.5)
    move (steps) steps
end
```

**How to build it step by step:**
1. Events → `when green flag clicked`
2. Pen → `erase all` (clears old drawings)
3. Pen → `pen up`, Motion → `go to x: 0 y: 0`, Pen → `set pen size to 2`, Pen → `pen down`
4. Variables → Make a Variable → name it `steps`, then Variables → `set steps to 0` (add after `pen down`)
5. Control → `repeat 200`
6. Inside the loop:
   - Motion → `move 1 steps`
   - Motion → `turn right 15 degrees` → change 15 to **61** (say: "61 degrees — not 60. That one degree makes it a spiral instead of a hexagon. Math is sneaky.")
   - Pen → `change pen color by 1`
   - Variables → `change steps by 0.5`
   - Motion → `move [steps] steps` (drag the `steps` variable into the move block)

**Press the green flag.** A colorful spiral blooms across the screen.

**React and riff (1 min):**
- "That's 12 blocks. No Photoshop, no drawing tablet. Just math and loops."
- Change the turn angle from 61 to 91 and run again — completely different pattern. "One number changes the whole thing."
- Change it to 121 — another pattern. "This is called generative art. Artists sell this stuff as NFTs and gallery prints."
- Change the repeat from 200 to 500 for a denser pattern.

**Key CS tie-in:** "This is the same `repeat` loop you used in your game. Same building blocks — totally different result."

**Instructor notes:**
- You must create the `steps` variable before building the loop. It's easy to forget this when live-coding.
- If the drawing is slow, reduce the repeat count to 100.
- The magic numbers: 61° gives a 60-petal spiral. 91° gives a square spiral. 121° gives a triangle spiral. Any non-factor of 360 produces a spiral; factors of 360 produce closed polygons.
- **Pre-build this project beforehand** and test it so you're confident with the block order. Have the finished project saved as a backup in case the live build goes sideways.

---

#### Demo 2: Beat Maker / Drum Machine (8 min)

**What they'll see:** An 8-pad drum machine where each sprite plays a different sound when tapped — a playable instrument built live.

**Setup (30 sec):**
1. Open a new Scratch project.
2. Delete the cat sprite.

**Build live (5 min) — talk as you go:**

Say: "Okay, art is cool. But what about music? Let's build a drum machine."

**Step 1: Create the first drum pad (2 min)**
1. Paint a new sprite: tap the sprite paintbrush icon → draw a colored square (or circle). Make it big — about 80×80. Choose a bold color (red).
2. Name it "Kick" (tap the sprite name field).
3. Go to the **Sounds** tab → **Choose a Sound** → search for "drum" → pick "Bass Drum" (or any drum hit).
4. Build the code:

```
when this sprite clicked
play sound [Bass Drum] until done
change size by (20)
wait (0.1) seconds
change size by (-20)
```

Say: "Tap it." *Tap the sprite.* It plays the drum hit and does a quick 'pulse' animation. "See that? Three extra blocks and it *feels* like a real button."

**Step 2: Duplicate to make 4 pads (2 min)**
1. Long-press the Kick sprite → **Duplicate**. Rename to "Snare".
2. Change its color in the costume editor. Change its sound to "Snare Drum".
3. Drag it to a different position on the stage.
4. Repeat: make "Hi-Hat" (with cymbal sound) and "Clap" (with clap sound).
5. Arrange the 4 pads in a 2×2 grid.

Say: "Long-press, duplicate, change the sound, change the color. That's it. Four instruments in under a minute."

**Step 3: Add a backdrop label (30 sec)**
1. Tap the backdrop → Paint → add text "TAP TO PLAY" at the top.

**Step 4: Play it! (1 min)**
- Tap the pads to play a beat. Get a rhythm going.
- Invite a learner to come up and play it. "Who wants to try?"
- If time allows, ask: "What sound would YOU add?" → show how to add a new sprite with a different sound in 15 seconds.

**React and riff (30 sec):**
- "Every music app on your phone works like this — buttons that trigger sounds. You just built the same thing."
- "If you had 8 pads and added a `forever` loop with a timer, you'd have a step sequencer — that's how GarageBand works under the hood."

**Key CS tie-in:** "Each pad is a sprite with its own code. That's parallelism — the same idea from Activity 1 where multiple sprites acted independently. Same concept, totally different application."

**Instructor notes:**
- **Pre-build this project beforehand.** Duplicating 4 sprites, renaming, and changing sounds live takes practice. Have a finished version saved as backup.
- The "pulse" animation (`change size by 20` → `wait` → `change size by -20`) is the hook — it makes it *feel* like a real instrument. Don't skip it.
- Good Scratch sound picks: Bass Drum, Snare Drum, Hi-Hat, Clap, Crash Cymbal, Conga, Bongo, Tambourine.
- If you want a wow moment, add a 5th pad with the **Text to Speech** extension and use `speak [yo!]` instead of a drum sound.
- On iPad, sound playback may have a slight delay on the first tap (browser audio policy). Tap each pad once before the demo to "warm up" the audio.

---

### Block 3: Create & Celebrate (3:00–3:30)

#### Activity 3: Creative Remix Challenge (3:00–3:20) — 20 min

**Goal:** Open-ended creative time to apply everything they've learned.

> **Choose your challenge:**
>
> **Option A — Remix:** Take your game from Activity 2 and add a major new feature:
> - A start screen with instructions
> - Multiple levels (speed up after every 10 points)
> - A second player controlled by keyboard
> - Custom sprite art (use the paint editor)
>
> **Option B — Fresh Build:** Start a new project of your choice:
> - A quiz game
> - An interactive music maker (expand on the drum machine demo!)
> - A virtual pet
> - An animated greeting card
> - A generative art piece (try different turn angles!)
> - Anything else you can imagine
>
> **Option C — Explore:** Browse the Scratch community (scratch.mit.edu/explore) for a project you think is cool. Tap "See Inside" to look at the code. Try to understand how one feature works, and explain it to a neighbor.
>
> **Option D — Remix a Demo:** Open the generative art or beat maker project your instructor just built (shared in the class). Tap "See Inside", then "Remix" to make your own version. Change the turn angle, add pads, mash them together — go wild.

**Instructor notes:**
- This is creative exploration time. Your main job is to walk around, encourage, and help unblock.
- Encourage learners to use the "See Inside" feature on community projects to learn from others' code — this is how real programmers learn.
- **Managing the energy dip:** By 3:00, some teens will be tired. Option C (explore the community) is a lower-energy path for learners who are fatigued. Don't force everyone into building mode. The demos you just did should have re-energized most of the room — point learners who are inspired by them toward Options B or D.
- **Spotting showcasers early:** As you walk around during this activity, mentally note 3–4 projects that would be fun to showcase. Ask those learners: "Would you be willing to show your project at the end?" Giving them advance notice reduces stage fright.
- **If a learner says "I'm done":** They're usually not — they just ran out of ideas. Try: "That's awesome. Now, what would make it 10x cooler?" or "Show me one thing you're most proud of in your code."

#### Showcase & Wrap-Up (3:20–3:30) — 10 min

1. **Gallery walk** (5 min)
   - Have 4–5 volunteers share their screen (or walk around the room to see each other's projects).
   - Quick applause / positive feedback after each demo.
   - **Instructor note:** Keep feedback specific: "I love how you made the sprite speed up — that shows you understand variables" lands better than "Great job." Connecting their work to CS concepts reinforces the learning without feeling like a lecture.

2. **Wrap-up discussion** (3 min)
   - *What was your favorite thing you built today?*
   - *What's one CS concept you'll remember?*
   - *What would you build if you had more time?*

3. **What's next?** (2 min) — Give learners a path to keep going:
   - **Keep using Scratch**: scratch.mit.edu — their projects are saved to their account.
   - **Scratch tutorials**: scratch.mit.edu/ideas — guided projects to try at home.
   - **Level up to text code**: 
     - Code.org (free courses for teens)
     - Khan Academy (JavaScript intro)
     - Python via Replit.com (free, works on iPad)
   - **CS careers**: Point out that CS isn't just about being a programmer — it's used in music, art, medicine, sports, gaming, fashion, and more.

---

## Concepts Covered (Summary)

| CS Concept | Where it was taught | Scratch blocks used |
|---|---|---|
| Sequencing | Activity 1 (animation) | Stacking blocks top-to-bottom |
| Events | Activity 1 | `when green flag clicked`, `when this sprite clicked` |
| Loops | Activity 2 (game) | `forever`, `repeat` |
| Conditionals | Activity 2 (game) | `if <> then`, `if <> then / else` |
| Variables | Activity 2 (game) | `score`, `lives`, `set`, `change` |
| Parallelism | Activity 1 (multiple sprites) | Multiple `when green flag clicked` stacks |
| Debugging | Pair testing | — (process, not a block) |
| Decomposition | Icebreaker + all activities | Breaking projects into sprite behaviors |
| Abstraction | Wrap-up discussion | Custom blocks (optional advanced) |
| Layering | Activity 1 & 2 | `go to front layer`, `go backward 1 layers` |
| Pen / Extensions | Live demo (generative art) | `pen down`, `change pen color`, `erase all` |

---

## Troubleshooting

| Issue | Solution |
|---|---|
| Scratch won't load on iPad | Make sure Safari is updated. Try clearing cache. Fallback: install the free Scratch app from App Store. |
| Blocks won't drag | Tap-and-hold, then drag. If using a stylus, make sure palm rejection is on. Sometimes rotating the iPad to landscape helps. |
| "My code doesn't work" | Check for a hat block (event block) at the top. Check which sprite is selected. Click the green flag. |
| Project didn't save | Scratch auto-saves when signed in. If not signed in, use File → Save to your computer to download the .sb3 file. |
| Wi-Fi is slow | Have learners work offline in the Scratch iPad app. They can upload projects later. |
| Learner is bored / too advanced | Challenge them to explore the Scratch community, remix a popular project, or try the "Extensions" menu (pen drawing, text-to-speech, translate). |
| Learner is frustrated / stuck | Pair them with a neighbor. Reduce scope: "Just make one sprite do one thing." Celebrate small wins. |

---

## Materials Checklist

- [ ] iPads (1 per learner, charged, set to **landscape orientation**)
- [ ] Reliable Wi-Fi
- [ ] Projector or shared display for demos
- [ ] Scratch class account with student credentials
- [ ] Printed login credentials (1 per learner)
- [ ] **Student Activity Guides** (1 per learner, printed or shared digitally)
- [ ] Scratch cheat sheets (optional, 1 per pair)
- [ ] Whiteboard or flip chart + markers
- [ ] Timer (phone or projected)
- [ ] A backup object for the icebreaker (marker, stuffed animal, etc.)
- [ ] 2–3 spare iPads with the **Scratch app** pre-installed (fallback for login issues)
