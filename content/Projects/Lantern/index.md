---
title: "Lantern of Souls"
summary: "AI Behavior Designer"
weight: 1
showHero: true
heroStyle: "big"
---
UE 5, Blueprints, C++

Lantern of Souls is a stealth horror game where you play as a Soul Guardian, tasked with guiding a Soul to ascension through a dark underworld full of corrupted spirits. Sneak, hide, use abilities, and move carefully through the level in order to prevent the terrifying Guards from detecting the Soul's light.

On this project, I'm primarily working on designing the behavior of the Guards, our intelligent enemy that hunts the player and the Soul. This project is ongoing and will be shipped in Spring 2027.


{{< feature-grid columns="3" >}}
  {{< feature title="Enemy Behavior" url="#enemy-behavior-and-movement" label="Enemy Behavior" >}}{{< /feature >}}
  {{< feature title="Designing the Horror Experience" url="#designing-the-horror-experience" label="Designing the Horror Experience" >}}{{< /feature >}}
  {{< feature title="Early Prototyping and Development" url="#early-prototyping-and-development" label="Early Prototyping and Development" >}}{{< /feature >}}
{{< /feature-grid >}}
---
## Enemy Behavior and Movement

| ![Describe the image](section-left.jpg) | **Enemy State Tree**<br>I designed and prototyped enemy state trees involving patrol, investigate, and aggro behavior states.|
| --- | --- |

| **Zone Manager**<br>I created a level-wide movement system where the Guards randomly select an empty "zone" and then choose a random point inside that zone to travel to. They then continue to visit the next closest point until all points in the zone have been visited. They then choose a new empty zone to go to and the process repeats. This allows for somewhat randomized but still rational, telegraphed behavior for the enemy. | ![Gif of Guards moving around a basic level, choosing new waypoints and zones](section-right.jpg) |
| --- | --- |

| ![Investigate Behavior GIF](section-left.jpg) | **Investigate Behavior**<br>Using Unreal 5 State Tree, I created an investigative behavior system where after losing sight of the player, the guard investigates points in the surrounding area, including wall cracks that could trigger a quick time event. |
| --- | --- |

| **Event Points**<br>I created colliders that have a chance to trigger spooky character moments for the enemy AI. Examples include pausing and looking around, scraping the walls, or peering around corners. These events contribute to the ambiance and scariness of the enemies. | ![Event Point GIF](section-right.jpg) |
| --- | --- |


---
## Designing the Horror Experience

| ![Temporary Rig GIF](guardrigdemo.gif) | **Temporary Rig**<br>In our early whitebox stage, I realized that I needed animations in order to test the emotional effect of certain enemy-player experiences. I created a simple but complete temporary rig to use for testing some pre-vis animations. |
| --- | --- |

| **Death Cutscene**<br>I directed animators in using the temporary rig to create the death cutscene animation test. I planned out the scene and created the fixed camera. | ![Death Cutscene GIF](section-right.jpg) |
| --- | --- | 

| ![Guard turning to look at player GIF](section-left.jpg) | **Guard Looking at Player**<br>Using the animation blueprint, I set up the guard's ability to look in the direction of the player when the player is detected. |
| --- | --- |


---
## Early Prototyping and Development

| **Distraction Throw**<br>I designed the mechanic for the player throwing a distraction to divert the enemy. | ![Distraction Throw GIF](section-right.jpg) |
| --- | --- |

| ![Old QTE GIF](section-left.jpg) | **Prototype QTE**<br>During the iteration process, I created early versions of the quick-time-event that occurs when the enemy searches a crack the player is hiding in. |
| --- | --- |


---
## Key Takeaways

**What Went Well**
I've loved working on enemy behavior for this game, and 

**What Went Wrong**


**What I Learned**
In addition to learning the technical skill of working with UE 5 and state trees in particular, this project has taught me to think about the player experience before anything else. I've learned to design around specific feelings I want to invoke in the player: in this game, both intense fear and relief. I've also learned to approach each itteration loop with a specific question to answer.