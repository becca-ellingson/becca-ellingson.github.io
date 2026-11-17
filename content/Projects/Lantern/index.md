---
title: "Lantern of Souls"
summary: "AI Behavior Designer"
weight: 1
showHero: true
heroStyle: "big"
---

Lantern of Souls is a stealth horror game where you play as a Soul Guardian, tasked with guiding a Soul to ascension through a dark underworld full of corrupted spirits. Sneak, hide, use abilities, and move carefully through the level in order to prevent the terrifying Guards from detecting the Soul's light.

This project is ongoing and will be shipped in Spring 2027.

Working on the guards


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

| ![Describe the image](section-left.jpg) | **Investigate Behavior**<br>Using Unreal 5 State Tree, I created an investigative behavior system where after losing sight of the player, the guard investigates points in the surrounding area, including wall cracks that could trigger a quick time event. |
| --- | --- |

| **Event Points**<br>I created colliders that have a chance to trigger spooky character moments for the enemy AI. Examples include pausing and looking around, scraping the walls, or peering around corners. These events contribute to the ambiance and scariness of the enemies. | ![Describe the image](section-right.jpg) |
| --- | --- |


---
## Designing the Horror Experience


| ![Describe the image](section-left.jpg) | **Subheading**<br>Description goes here. |
| --- | --- |

| **Subheading**<br>Description goes here. | ![Describe the image](section-right.jpg) |
| --- | --- | 

| ![Describe the image](section-left.jpg) | **Subheading**<br>Description goes here. |
| --- | --- |


---
## Early Prototyping and Development

| **Subheading**<br>Description goes here. | ![Describe the image](section-right.jpg) |
| --- | --- |

| ![Describe the image](section-left.jpg) | **Subheading**<br>Description goes here. |
| --- | --- |

| **Subheading**<br>Description goes here. | ![Describe the image](section-right.jpg) |
| --- | --- |

