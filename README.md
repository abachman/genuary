# genuary 2022

sketches in code.

- _day 01_
- _day 02_
- [day 03](#2022-01-03)
- [day 04](#2022-01-04)
- [day 05](#2022-01-05)
- [day 06](#2022-01-06)
- [day 07](#2022-01-07)
- [day 08](#2022-01-08)
- [day 09](#2022-01-09)
- [day 12](#2022-01-12)
- [day 13](#2022-01-13)
- [day 14](#2022-01-14)
- [day 15](#2022-01-15)
- _day 16_
- [day 17](#2022-01-17)
- _day 18_
- [day 19](#2022-01-19)
- [day 20](#2022-01-20)

## rules

for me, not for you

1. clean editor.p5js.org window
1. 400x400 area
1. ~~still images~~ (broken by day 6)
1. [link to sketch code](https://editor.p5js.org/abachman/collections/P-ovJH5BB)
1. write code on p5js.org in-browser, edit README in-browser, tweet from phone

### 2022-01-03

arrow diagrams. (i didn't read the instructions 🤷‍♂️)

[sketch](https://editor.p5js.org/abachman/full/Eu_KjU34d)

![diagrams-2022-01-03](https://user-images.githubusercontent.com/13002/147996628-9af6a2a8-b66e-4eb4-a5cc-4090b000c7c7.png)
![diagrams-2022-01-03--002](https://user-images.githubusercontent.com/13002/147996701-4f8e20fa-c093-4a21-8abb-4a2e5cdb393e.png)

### 2022-01-04

actually [read the prompt](https://genuary.art/prompts#jan4) today! saw "fidenza" and just did some [flow fields](https://editor.p5js.org/abachman/full/N1QAqnwMA)

![flow-field-003](https://user-images.githubusercontent.com/13002/148117162-ab72c4d8-8e19-43ea-be2d-35ffac1a48d2.png)
![flow-field-004](https://user-images.githubusercontent.com/13002/148117167-fe7218f2-0250-4edc-b933-47105af77b2a.png)

re-read the prompt and saw "next next [Fidenza](https://tylerxhobbs.com/fidenza)" so I went somewhere else. the next next fidenza probably won't be flow fields, i like cellular automata so why not? 

scratch rewrote some ["Langston's Ant"](https://en.wikipedia.org/wiki/Langton%27s_ant) code that i worked on with my son recently so that it would auto-generate rule sets and save everything it drew. cellular automata like these are interesting because they may be a closer representation to how the universe is built than anything else that can be summed up in fewer rules than you can count on one hand. the system is turing complete. complex behavior arises from simple rules. future states cannot be predicted without calculating from the present. "undecidability." very small changes in the rules produce wildly different outcomes.

sounds like fertile ground for future exploration! 

i'm lazy so no iteration on palette or cell size here. provisions made for fiddling with that stuff, tho. [here's a link to the sketch so you can make your own dumb NFTs or whatever](https://editor.p5js.org/abachman/sketches/5fsl7jhoj).

ruleset: LLLR

![ant-life-LLLR](https://user-images.githubusercontent.com/13002/148147897-91adeb9a-bf15-401d-a6e2-05aea789c011.png)

ruleset: LRLLLLR

![ant-life-x1-LRLLLLR](https://user-images.githubusercontent.com/13002/148151633-218ca7f5-0e53-41a9-b4d3-d99212e9b783.png)


### 2022-01-05

prompt: 'destroy a square' 

kept it clean, translate - rotate - line. tweak for variation. i started out cutting the square into pieces with scattered lines, found i liked the layering better. getting random 

[sketch](https://editor.p5js.org/abachman/sketches/u-EBIyXf-)

centralized / starlike (no jitter on x, y)

![2022-01-05--square--16ff64-40-100-200-0011-6283--226](https://user-images.githubusercontent.com/13002/148301123-cfc5760c-4eed-47ab-be75-70eb05e2b21a.png)
![2022-01-05--square--18ff64-40-100-200-0011-6283--3965](https://user-images.githubusercontent.com/13002/148301114-4e66182c-c675-435e-9b88-784e5648c377.png)

grassy field (small rotation jitter, color stable)

![2022-01-05--square--00ff64-40-0-0 5-1111-500--266](https://user-images.githubusercontent.com/13002/148301175-9870274e-5bae-48b3-b244-da037b62ea91.png)

galactic super clusters (full jitter on x,y & rot, color stable)

![2022-01-05--square--00ffff-40-0 15-0 1-1110-6283--1530](https://user-images.githubusercontent.com/13002/148301659-1d0dbde8-58ce-4d29-882c-ee39c470b9f8.png)

### 2022-01-06

light painting. based on works by my friend [Joshua Penrose](https://joshuapenrose.com/untitled-light-paintings-triptych). "trade"?, nah, "borrow"

[sketch](https://editor.p5js.org/abachman/sketches/jKtcd_X2u)

wanted to play with framed movement. p5js image `filter(BLUR, 4)` is probably a lot slower than a custom shader would be. will have to poke at shaders sometime soon. used the [ccapture](https://peterbeshai.com/blog/2018-10-28-p5js-ccapture/) library to create a video for this one.

- [light painting video .mp4](https://user-images.githubusercontent.com/13002/148457559-3528f0fe-5b1d-49a6-ad5f-96b9e7a58461.mp4)

![light-painting--still-01](https://user-images.githubusercontent.com/13002/148460016-01623ddb-8878-40bb-a3f1-15822e260d18.png)
![light-painting--still-02](https://user-images.githubusercontent.com/13002/148460049-c002ebf6-47a1-46dc-83ff-8cdc756567e2.png)

### 2022-01-07

"sol lewitt drawings"

took the rules, left the lines. went with an 'old reliable' random walk painting system. tweakable color and counts.

```
100 people gather on an empty lot
each carries one can of paint and should
  paint the spot they are standing on
  turn in a random direction
  step forward
repeat until 5000 steps have been taken
```

[sketch](https://editor.p5js.org/abachman/full/yFWAuwlno)

monochrome: 

![sol-lewitt--5000-100-1 2_3-0_20-40_70-80_100](https://user-images.githubusercontent.com/13002/148603288-587a2457-6076-48b6-afa5-bf7f76006cd7.png)

color blasted:

![sol-lewitt--5000-100-1 2_3-0_256-100_100-100_100](https://user-images.githubusercontent.com/13002/148603199-32abcb17-6a5d-481e-9b62-6d7a8564d107.png)


### 2022-01-08

"single curve only"

what if you had a marker that never dried out and an arm that never stopped moving?

go-pro style footage of an epic coloring session

[sketch](https://editor.p5js.org/abachman/sketches/82kNk-PDD)

[moving image .mp4](https://user-images.githubusercontent.com/13002/148667362-fbeec504-9f57-49a2-97a6-227a06298070.mp4)

visible canvas (400x400)

![visible canvas](https://user-images.githubusercontent.com/13002/148667375-e0bd6cac-36e8-44bc-91eb-6de92c553711.png)

full canvas (2000x2000)

![continuous-curve--5177](https://user-images.githubusercontent.com/13002/148667380-9bf3cbbf-1281-44bd-8cbf-f4c58348a96d.jpg)

### 2022-01-09

a text-based tribute to one of my favorite quotes about programming, by Fred Brooks. i took massive liberties with whitespace here: 

```
  The programmer, like the poet
  works only slightly removed
  from pure thought stuff.
  They build their castles
  in the air, from air,
  creating by exertion
  of the imagination.
  Few media of creation
  are so flexible,
  so easy to polish and rework,
  so readily capable of realizing
  grand conceptual structures.
  The magic of myth and legend
  has come true in our time.

Fred Brooks, 
"The Mythical Man Month"
```

[sketch](https://editor.p5js.org/abachman/full/1tAwG0BIj)

![air-architects--2022-01-09-02](https://user-images.githubusercontent.com/13002/149052158-87ec8829-91bd-4e61-997b-f84d37470bc6.png)

simple, but the end result of playing with colors, lerping colors (not really possible in HSB), palette generation, moving things, multiple layers, and aliasing artifacts. play is important and most doesn't go anywhere useful. whether this sketch went anywhere useful at all is super debateable :)  

### 2022-01-12

"packing"

i wanted to see circle packing two ways: just the circles, just the touches. 

[sketch](https://editor.p5js.org/abachman/full/7aDENmg7o) has some fun parameters for initial seeding, spawn rate, growth rate that change the balance of sizes.

just the circles

![circle-packing--circles](https://user-images.githubusercontent.com/13002/149267661-1a36ec98-6bc9-492a-82a3-29b9b5ed9d7b.png)

just the lines

![circle-packing--lines](https://user-images.githubusercontent.com/13002/149267688-e72ad3c1-f214-424d-be21-5d9b708bc1ed.png)

### 2022-01-13

like anytime i'm grasping for something to put on a blank screen, how about conway's game of life?

[sketch](https://editor.p5js.org/abachman/full/y1FrVDp4g)

[moving image .mp4](https://user-images.githubusercontent.com/13002/149409823-356818e9-c11a-40b0-b968-3d9fccaa298b.mp4)

### 2022-01-14

"Something you’d never make."

this one made me feel dirty. both for the integrated qr code and the reference to the [environment killing ponzi scheme](https://everestpipkin.medium.com/but-the-environmental-issues-with-cryptoart-1128ef72e6a3) that is NFTs.

[sketch](https://editor.p5js.org/abachman/full/jI2UD0iiN)

[moving image .mp4](https://user-images.githubusercontent.com/13002/149605874-5b40ec3f-0cf0-4b5a-a53b-167ab40eec82.mp4)


### 2022-01-15

"Sand"

i wanted to play with a high-count particle system that could animate, but also keep around 10k+ particles. got that with a background + foreground separation w/ createGraphics for points that have finished moving and particle list for points still in motion.

also needed an interesting movement pattern and stumbled on [lissajous curves](https://en.wikipedia.org/wiki/Lissajous_curve)

[sketch](https://editor.p5js.org/abachman/full/3OubqYGg2)

![sand-tracing--2022-01-15](https://user-images.githubusercontent.com/13002/149640526-b19250d3-2625-429f-9253-69a7badcb4ea.png)

[moving image mp4](https://user-images.githubusercontent.com/13002/149640539-6d5f5b5c-d271-4463-be58-a0a8618f2ba4.mp4)

### 2022-01-17

"three colors" [sketch](https://editor.p5js.org/abachman/full/dRXT5CdFy)

i played with the color wheel, lots of tweaking of color selection, brightness and saturation selection, and motion. also first time playing with p5.js' DOM manipulation tools. handy for controls.

didn't make a video because _lazy_.

![color-wheeling--2022-01-17](https://user-images.githubusercontent.com/13002/149856636-3315e546-8ade-4443-967c-5d9619e4a8d5.png)


### 2022-01-19

"use text/typography"

textToPoints + atan2 + color smoosh

[sketch](https://editor.p5js.org/abachman/full/A8toulllC)

[video file](https://user-images.githubusercontent.com/13002/150455964-874dec7f-f913-4e08-a48d-f6054586cb86.mp4)


### 2022-01-20

"sea of shapes" -> but i'm going with "shapes of the sea"

[stealing from myself](https://github.com/abachman/genuary/blob/main/offshoots.md#blob-circles--gems--splats) with accidental diatoms

![image of circle splats](https://user-images.githubusercontent.com/13002/150049813-ccbf3c89-8a3b-46ab-993b-c2af17e16af2.png)
