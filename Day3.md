# Day 3 - Pixel-based Drawing

## Prepare

Look at a job listing. Here's one at [Media Molecule](https://www.mediamolecule.com/jobs/), maker of Little Big Planet ([or here for an archived pdf](./MediaMoleculeJobPosting.pdf)). Look for the skills they want (hard and soft) and what application materials they want.

- Skills
  - Programmer
  - C++ (Notice they write their own engine, they're not using Unity/Unreal/Whatever)
  - Teamwork
  - Past Experience - Example of Polished Game
  - Math
  - C++ (again!!!)
  - Programming Architecture
  - Data structures

- Application
  - Portfolio or Showreel



## See

[Name that game](https://github.com/CS2510/games/blob/master/NameThatGame.pptx) to see how much you can tell about a game just from its UI. I've taken games from IGN's top 100 games and blacked out the UI. Can you tell just from looking at the location of the UI what the genre is? How come? When you write a game, you want your player to feel very comfortable with your game--make sure your UI layout is as familiar to them as these classic games.

## Code

If we're going to make a game, we need to draw on the screen. There are two ways to do this.

### Two ways to represent an image

- Pixel-based (Editors include Photoshop, MS paint, Gimp)

Is "intuitive" when you are coming from a screen. You assign each pixel a color.

Great: It is easy to represent a photograph and fast to send pixel data to a screen.

Problems: Doesn't scale (it gets jagged) and you can't edit it logically.

- Vector-based (Editors include Illustrator, Inkscape, PowerPoint)

Great: Vector-based images scale infinitely

Problems: It is hard to represent a photograph and slow to send data to screen since vector images  need to be rendered.

- In HTML/CSS/JS

Pixel-based drawing is done on a `<canvas>`

Vector-based drawing is done within a `<svg>`

We'll start with a pixel-based drawing on a `<canvas>`

### Two ways to draw

When you draw, you need to tell the computer both the color and location of the draw call. There are two approaches to doing this, and they tend to be language specific. When you draw with code, you need to know which approach the language/library/api uses.


- Stateful drawing 

Color calls and location of draw are made in separate calls. For example: All future calls will be red. Draw a line. (e.g. Java, JS)

- Stateless drawing

Color calls and location of draw are made in the same call. For example: Draw a red line. (Microsoft-centric approach, e.g. c#, Win32)

### Colors representation in javascript

You can represent colors three ways in HTML/CSS/JS

- [Web Colors](https://en.wikipedia.org/wiki/Web_colors)
- Hex #RRGGBB
- rgb(0-255,0-255,0-255)

I've found it helpful to pick a color pallette using one of many online tools, for example: [paletton.com](http://paletton.com)
