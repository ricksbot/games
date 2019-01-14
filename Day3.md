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

[Name that game]("./Name that game.pptx") to see how you can tell about a game just from its ui. I've taken games from IGN's top 100 games and blacked out the UI. Can you tell just from looking at the location of the UI what the genre is? How come? When you write a game, you want your player to feel very comfortable with your game--make sure your UI layout is as familiar to them as these classic games.

## Code

### Two ways to draw

- Pixel-based (Photoshop, MS paint, Gimp)

Is "intuitive" when you are coming from a screen. You assign each pixel a color.

Problems: Doesn't scale and you can't edit logically.

Great: photographs and great to send to the screen.


- Vector-based (Illustrator, Inkscape, PowerPoint)

Great: scale infinitely

Problems: Terrible for photographs, time consuming to map to a screen.


Back to HTML/JS
Pixel-based drawing is done on a `<canvas>`

Vector-based drawing is done within a `<svg>`

### Two ways to draw

Stateful drawing - All future calls will be red. Draw a line. (e.g. Java, JS)

Stateless drawing - all information (about color) included in all drawing calls. (Microsoft-centric approach, e.g. c#, c++)

### Colors in javascript

- Strings
- Hex #RRGGBB
- rgb(0-255,0-255,0-255

http://paletton.com
