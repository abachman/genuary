# genuary 2022

sketches in code.

- [day 03](#2022-01-03)
- [day 04](#2022-01-04)
- [day 05](#2022-01-05)
- [day 06](#2022-01-06)
- [day 07](#2022-01-07)

## rules

for me, not for you

1. clean editor.p5js.org window
1. 400x400 area
1. ~~still images~~ (broken by day 6)
1. [link to sketch code](https://editor.p5js.org/abachman/collections/P-ovJH5BB)

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



