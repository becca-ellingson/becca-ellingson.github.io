---
title: "Solar Simulator"
summary: "Solar system"
weight: 2
showHero: true
heroStyle: "big"
---
UE 5, Blueprints

Inspired by some of my favorite games, Outer Wilds and Super Mario Galaxy, I wanted to create a customizable small scale solar system and planetary gravity system that the player could explore and fly around. This solo project was extremly enjoyable to make, and I plan to re-visit it in the future.

{{< feature-grid columns="3" >}}
  {{< feature title="Planetary Gravity System" url="#planetary-gravity-system" label="Planetary Gravity System" >}}{{< /feature >}}
  {{< feature title="Customizable Solar System" url="#customizable-solar-system" label="Customizable Solar System" >}}{{< /feature >}}
{{< /feature-grid >}}
---
## Planetary Gravity System

| **Walking on Planet Gravity**<br>I created a system where the player can walk, run, and jump all the way around a small planet. The camera constantly adjusts to the player's new "up" direction.| ![Describe the image](section-right.jpg) |
| --- | --- |

| ![Describe the image](section-left.jpg) | **Flying in Zero-G**<br>The player can fly from planet to planet, affected by gravity only if they are within the planet's gravity radius. |
| --- | --- |

| **Speed Boosts**<br>Flying is made more enjoyable by controls to rapidly speed up and slow down. FOV changes during acceleration and deceleration create a sense of momentum. | ![Describe the image](section-right.jpg) |
| --- | --- | 

| ![Describe the image](section-left.jpg) | **Omnidirectional Flying**<br>Flying is omnidirectional, and the player can rotate their camera to any angle in order to orient themselves in space. |
| --- | --- |


---
## Customizable Solar System

| **Planets Orbit Each Other**<br>Solar systems are completly customizable, and a user can create new planets and set them to orbit one another in the drop down menue. Planets will automatically make circles around the planet they are set to orbit at the distance they are placed away from it. | ![Describe the image](section-right.jpg) |
| --- | --- |

| ![Describe the image](section-left.jpg) | **Customizable Orbital/Rotational Period, size, and gravity**<br>Orbital and rotational period are both customizable, as are planet size and planet gravity. Though I initially considered syncing gravity automatically with planet scale, I realized that would leave me with only a small range of planet sizes that are playable. Players found it more enjoyable to have slightly less realistic physics, with tiny planets having disproportionatly large gravity and large planets not having so much gravity as to trap the player and prevent them from leaving. |
| --- | --- |


---
## Key Takeaways

### What Went Well:
As someone with a passion for astronomy, I loved working on this project. I especially enjoyed creating the customizable solar system, since sandbox space games are something that really interests me. I also thought the flying mechanic ended up feeling really good, even though I was worried at the start of the project that omnidirectional flying would feel clunky and confusing.

### What Went Wrong:
This was one of my earlier projects in Unreal Engine, and my code quality makes that obvious. My blueprints are unorganized and have way too many dependancies, and if I were to re-do this project I'd architect it better and base all of my classes in c++. I'd also create my own character movement component with my own custom physics, rather than constantly have to disable and fight the default UE5 character movement componant.

### What I Learned:
My primary takeaway from this project is that while many default systems can be re-used and adapted to a project's needs, it's better to consider from the beginning if those systems actually contribute meaningfully to the game. Using built in systems needs to be a conscious choice, not the default, and it's often better to design something myself that fits my project exactly, rather than fighting something not made for what I'm working on.
