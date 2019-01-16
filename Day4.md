# Day 4

## Quick Review

Difference between GUI and !GUI.

Make your game comfortable with a comfortable GUI.

## GUI Layout

GUI uses screen coordinates.

+X From left (0) to right (width.)

+Y From Top (0) to bottom (height)

### Problems

- Problem #1: People don't think in terms of pixels from the upper left corner. (Not even programmers.)

- Problem #2
    - Early consoles had a resolution of 449x483 
    - Widescreen
        - 2048x[Unspecified]
        - 1920x1200
        - 1920x1080
        - 1280x720
    - Computers
        - 640x480
        - 800x600
        - 960x720
        - 1024x768
        - 1280x960
        - 1400x150
        - 1440x1080
        - 1600x1200
        - 1856x1392
        - 1920x1440
        - 2048x1536
    - Phones
        - on and on and on

### Solutions

Never, ever, ever, ever hard code your GUI..... Unless you are writing for a VERY specific product. i.e. You are writing emulated NES games for a nerdy club.

- Option 1: Use clipping Coordinates.

Clipping coordinates treats your screen as if:
- The center of your screen was at 0,0
- +x goes right.
- +y goes up.
- The smallest dimension in pixels (x or y) extends one unit in the positive and negative direction.

Benefits
- No reversed y axis
- Independent of pixels in display



- Option 2: Offset from Edges/Centers(e.g. horizontal)/Middles(e.g. vertically)

Define everything as so many pixels off from some anchor.

This element is anchored 10 pixels off the left side, 10 pixels off the right side, 10 pixels off the bottom, and is 50 pixels high.

- Option 3: Combine the two - So many clipping units off an anchor

This element is anchored .1 clipping units pixels off the left side, .1 clipping units pixels off the right side, .1 clipping units pixels off the bottom, and is .25 clipping units high.

In game engines, clipping units are often disguised as percentages.

## Code

The code that does takes this hybrid approach can be found here: [https://github.com/CS2510/code/blob/master/day4/index.html](https://github.com/CS2510/code/blob/master/day4/index.html).
