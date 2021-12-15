NMD 211 - 1001
 Date: 12/14/2021
 
 Task:  Iterative Art - Start with the picture you made in the 6th step of iterative art.
 
 Sorce/Inspiration: Actually, my inspiration was Watermelon Bubbies, the first game I ever pogrammed.
                    I just want to see if I can learn to program a better emote system where multiple conditions can effect
                    the emote of the sprite. I also want to see if I can make it look like the two bees have different personalities
                    since having multiple bees with the exact same reactions will appear flat and boring.
 
 Steps/Components: 1. Save As `lastname_firstname_iterative12'
 2. Spend the first 20 minutes of lab with this work. What can you do?
 - Add new shapes
 - Add motion
 - Add variables for everything
 - See if you can make anything you repeatedly do into a function or a class. Make it into a function or class.
 - Add new things. Add them normally, then change them into a function or a class.
 - Clean your code / comment
 3. After 20 minutes, save, zip, and submit this file.
 
 
 - Goal: Make two bees that react differently to each button you press.
 - Computer doesn't store files that well, so I personally resorted to keeping all the code in one tab. If you want though, you can move the sprite code into other tabs to keep better track of it. I highly reccommend it.
 - This was mainly to further push how expressive you can get with a few circles and ovals.
 
 */

int beeWidth = 200;
int white = 255;
int black = 0;

boolean emoteOne = false;            // overBee's emote funtions
boolean emoteTwo = false;
boolean emoteThree = false;
boolean emoteFour = false;
boolean emoteFive = false;
boolean emoteSix = false;
boolean emoteSeven = false;
boolean emoteEight = false;
boolean emoteNine = false;
boolean emoteTen = false;

boolean emoteA = false;                // subtleBee's emote funtions
boolean emoteB = false;
boolean emoteC = false;
boolean emoteD = false;
boolean emoteE = false;
boolean emoteF = false;
boolean emoteG = false;
boolean emoteH = false;
boolean emoteI = false;
boolean emoteJ = false;

void setup() {
  size (900, 500);                     // canvas
  background(70);
}

void draw () {
  background(70);
  addOverBee(200, 200);                //overly expressivebee
  addSubtleBee(500, 0);                //not as expressive bee

  if (keyCode == '1') {                // overBee's emote funtions
     emoteOne = true;
     emoteTwo = false;
     emoteThree = false;
     emoteFour = false;
     emoteFive = false;
     emoteSix = false;
     emoteSeven = false;
     emoteEight = false;
     emoteNine = false;
     emoteTen = false;
     
  } else {
  if (keyCode == '2') {
     emoteOne = false;
     emoteTwo = true;
     emoteThree = false;
     emoteFour = false;
     emoteFive = false;
     emoteSix = false;
     emoteSeven = false;
     emoteEight = false;
     emoteNine = false;
     emoteTen = false;
  } else {
    if (keyCode == '3') {
     emoteOne = false;
     emoteTwo = false;
     emoteThree = true;
     emoteFour = false;
     emoteFive = false;
     emoteSix = false;
     emoteSeven = false;
     emoteEight = false;
     emoteNine = false;
     emoteTen = false;
  } else {
    if (keyCode == '4') {
     emoteOne = false;
     emoteTwo = false;
     emoteThree = false;
     emoteFour = true;
     emoteFive = false;
     emoteSix = false;
     emoteSeven = false;
     emoteEight = false;
     emoteNine = false;
     emoteTen = false;
  } else {
    if (keyCode == '5') {
     emoteOne = false;
     emoteTwo = false;
     emoteThree = false;
     emoteFour = false;
     emoteFive = true;
     emoteSix = false;
     emoteSeven = false;
     emoteEight = false;
     emoteNine = false;
     emoteTen = false;
  } else {
    if (keyCode == '6') {
     emoteOne = false;
     emoteTwo = false;
     emoteThree = false;
     emoteFour = false;
     emoteFive = false;
     emoteSix = true;
     emoteSeven = false;
     emoteEight = false;
     emoteNine = false;
     emoteTen = false;
  } else {
    if (keyCode == '7') {
     emoteOne = false;
     emoteTwo = false;
     emoteThree = false;
     emoteFour = false;
     emoteFive = false;
     emoteSix = false;
     emoteSeven = true;
     emoteEight = false;
     emoteNine = false;
     emoteTen = false;
  } else {
    if (keyCode == '8') {
     emoteOne = false;
     emoteTwo = false;
     emoteThree = false;
     emoteFour = false;
     emoteFive = false;
     emoteSix = false;
     emoteSeven = false;
     emoteEight = true;
     emoteNine = false;
     emoteTen = false;
  } else {
    if (keyCode == '9') {
     emoteOne = false;
     emoteTwo = false;
     emoteThree = false;
     emoteFour = false;
     emoteFive = false;
     emoteSix = false;
     emoteSeven = false;
     emoteEight = false;
     emoteNine = true;
     emoteTen = false;
  } else {
    if (keyCode == '0') {        // subtleBee's emote funtions
     emoteOne = false;
     emoteTwo = false;
     emoteThree = false;
     emoteFour = false;
     emoteFive = false;
     emoteSix = false;
     emoteSeven = false;
     emoteEight = false;
     emoteNine = false;
     emoteTen = true;
  } else {
    
    if (keyCode == 'Q') {
     emoteA = true;
     emoteB = false;
     emoteC = false;
     emoteD = false;
     emoteE = false;
     emoteF = false;
     emoteG = false;
     emoteH = false;
     emoteI = false;
     emoteJ = false;
  } else {
    if (keyCode == 'W') {
     emoteA = false;
     emoteB = true;
     emoteC = false;
     emoteD = false;
     emoteE = false;
     emoteF = false;
     emoteG = false;
     emoteH = false;
     emoteI = false;
     emoteJ = false;
  } else {
    if (keyCode == 'E') {
     emoteA = false;
     emoteB = false;
     emoteC = true;
     emoteD = false;
     emoteE = false;
     emoteF = false;
     emoteG = false;
     emoteH = false;
     emoteI = false;
     emoteJ = false;
  } else {
    if (keyCode == 'R') {
     emoteA = false;
     emoteB = false;
     emoteC = false;
     emoteD = true;
     emoteE = false;
     emoteF = false;
     emoteG = false;
     emoteH = false;
     emoteI = false;
     emoteJ = false;
  } else {
    if (keyCode == 'T') {
     emoteA = false;
     emoteB = false;
     emoteC = false;
     emoteD = false;
     emoteE = true;
     emoteF = false;
     emoteG = false;
     emoteH = false;
     emoteI = false;
     emoteJ = false;
  } else {
    if (keyCode == 'Y') {
     emoteA = false;
     emoteB = false;
     emoteC = false;
     emoteD = false;
     emoteE = false;
     emoteF = true;
     emoteG = false;
     emoteH = false;
     emoteI = false;
     emoteJ = false;
  } else {
    if (keyCode == 'U') {
     emoteA = false;
     emoteB = false;
     emoteC = false;
     emoteD = false;
     emoteE = false;
     emoteF = false;
     emoteG = true;
     emoteH = false;
     emoteI = false;
     emoteJ = false;
  } else {
    if (keyCode == 'I') {
     emoteA = false;
     emoteB = false;
     emoteC = false;
     emoteD = false;
     emoteE = false;
     emoteF = false;
     emoteG = false;
     emoteH = true;
     emoteI = false;
     emoteJ = false;
  } else {
    if (keyCode == 'O') {
     emoteA = false;
     emoteB = false;
     emoteC = false;
     emoteD = false;
     emoteE = false;
     emoteF = false;
     emoteG = false;
     emoteH = false;
     emoteI = true;
     emoteJ = false;
  } else {
    if (keyCode == 'P') {
     emoteA = false;
     emoteB = false;
     emoteC = false;
     emoteD = false;
     emoteE = false;
     emoteF = false;
     emoteG = false;
     emoteH = false;
     emoteI = false;
     emoteJ = true;
     
  }}}}}}}}}}}}}}}}}}}}}

void addOverBee(float x, float y) {
  translate(x, y);
  if (emoteTen) {                                  
    noStroke();
    fill(120, 200, 255);
    circle(-68, 6, 160); //left wing
    fill(120, 200, 255);
    circle(68, 6, 160); //right wing
    fill(255, 255, 50);
    circle(0, 24, beeWidth); // bee's body
    fill(black);
    circle(-72, 0, 136); // left eye
    fill(black);
    circle(72, 0, 136); // right eye
    fill(white);
    circle(-72, 0, 52); // left iris
    fill(white);
    circle(72, 0, 52); // right iris
    fill(white);
    circle(-40, -20, 56); // left eyeshine
    fill(white);
    circle(104, -20, 56); // right eyeshine
    fill(white);
    circle(-44, 16, 16); // left eyeshine
    fill(white);
    circle(100, 16, 16); // right eyeshine
    fill(black);
    circle(0, 60, 32); // mouth                                
  } else if (emoteNine) {
    noStroke();
    fill(120, 200, 255);
    circle(-78, 96, 160); //left wing
    fill(120, 200, 255);
    circle(78, 96, 160); //right wing
    fill(255, 255, 50);
    circle(0, 24, beeWidth); // bee's body
    fill(black);
    circle(-90, 10, 36); // left eye
    fill(black);
    circle(90, 10, 36); // right eye
    fill(black);
    circle(17, 90, 32); // mouth
  } else if (emoteEight) {
    noStroke();
    fill(120, 200, 255);
    circle(-98, 36, 160); //left wing
    fill(120, 200, 255);
    circle(98, 36, 160); //right wing
    fill(255, 255, 50);
    circle(0, 24, beeWidth); // bee's body
    fill(black);
    circle(-82, -40, 176); // left eye
    fill(black);
    circle(82, -40, 176); // right eye
    fill(white);
    circle(-72, -40, 152); // left iris
    fill(white);
    circle(72, -40, 152); // right iris
    fill(200, 100, 200);
    ellipse(-94, 55, 56, 26); // left blush
    fill(200, 100, 200);
    ellipse(94, 55, 56, 26); // right blush
    fill(black);
    circle(0, 120, 22); // mouth
  } else if (emoteSeven) {
    noStroke();
    fill(120, 200, 255);
    circle(-68, -6, 160); //left wing
    fill(120, 200, 255);
    circle(68, -6, 160); //right wing
    fill(255, 255, 50);
    circle(0, 24, beeWidth); // bee's body
    fill(black);
    circle(-72, 10, 6); // left eye
    fill(black);
    circle(72, 10, 6); // right eye
    fill(200, 100, 200);
    ellipse(-94, 55, 56, 26); // left blush
    fill(200, 100, 200);
    ellipse(94, 55, 56, 26); // right blush
    fill(black);
    ellipse(0, 70, 132, 12); // mouth
  } else if (emoteSix) {
    noStroke();
    fill(120, 200, 255);
    circle(-68, 36, 160); //left wing
    fill(120, 200, 255);
    circle(68, 56, 160); //right wing
    fill(255, 255, 50);
    circle(0, 24, beeWidth); // bee's body
    fill(black);
    ellipse(-72, 90, 90, 12); // left eye
    fill(black);
    ellipse(72, 90, 90, 12); // right eye
    fill(black);
    circle(0, 120, 42); // mouth
  } else if (emoteFive) {
    noStroke();
    fill(120, 200, 255);
    circle(-68, 96, 160); //left wing
    fill(120, 200, 255);
    circle(68, 96, 160); //right wing
    fill(255, 255, 50);
    circle(0, 24, beeWidth); // bee's body
    fill(black);
    ellipse(-62, -40, 90, 12); // left eye
    fill(black);
    ellipse(62, -40, 90, 12); // right eye
    fill(black);
    ellipse(0, 60, 32, 114); // mouth
  } else if (emoteFour) {
    noStroke();
    fill(120, 200, 255);
    circle(-78, 76, 160); //left wing
    fill(120, 200, 255);
    circle(78, 76, 160); //right wing
    fill(255, 255, 50);
    circle(0, 24, beeWidth); // bee's body
    fill(black);
    ellipse(-62, 60, 90, 12); // left eye
    fill(black);
    ellipse(62, 60, 90, 12); // right eye
    fill(150, 170, 255);
    ellipse(-72, 75, 52, 23); // left tear
    fill(150, 170, 255);
    ellipse(72, 75, 52, 23); // right tear 
    fill(white);
    circle(-80, 70, 5); // left tear shine
    fill(white);
    circle(80, 70, 5); // right tear shine
    fill(black);
    circle(0, 90, 12); // mouth
  } else if (emoteThree) {
    noStroke();
    fill(120, 200, 255);
    circle(-68, -26, 160); //left wing
    fill(120, 200, 255);
    circle(68, -26, 160); //right wing
    fill(255, 255, 50);
    circle(0, 24, beeWidth); // bee's body
    fill(black);
    circle(-72, 0, 136); // left eye
    fill(black);
    circle(72, 0, 136); // right eye
    fill(white);
    circle(-72, 0, 102); // left iris
    fill(white);
    circle(72, 0, 102); // right iris
    fill(white);
    circle(-20, -20, 16); // left eyeshine
    fill(white);
    circle(124, -20, 16); // right eyeshine
    fill(black);
    ellipse(0, 60, 32, 64); // mouth
  } else if (emoteTwo) {
    noStroke();
    fill(120, 200, 255);
    circle(-68, 76, 160); //left wing
    fill(120, 200, 255);
    circle(68, 76, 160); //right wing
    fill(255, 255, 50);
    circle(0, 24, beeWidth); // bee's body
    fill(black);
    circle(-72, 0, 136); // left eye
    fill(black);
    circle(72, 0, 136); // right eye
    fill(white);
    circle(-72, 0, 52); // left iris
    fill(white);
    circle(72, 0, 52); // right iris
    fill(white);
    circle(-40, -20, 56); // left eyeshine
    fill(white);
    circle(104, -20, 56); // right eyeshine
    fill(white);
    circle(-44, 16, 16); // left eyeshine
    fill(white);
    circle(100, 16, 16); // right eyeshine
    fill(black);
    circle(0, 60, 32); // mouth
  } else if (emoteOne) {
    noStroke();
    fill(120, 200, 255);
    circle(68, -16, 160); //right wing
    fill(120, 200, 255);
    circle(-68, -16, 160); //left wing
    fill(255, 255, 50);
    circle(0, 40, beeWidth); // bee's body
    fill(black);
    circle(-72, 40, 120); // left eye
    fill(black);
    circle(72, 40, 120); // right eye
    fill(white);
    circle(-72, 40, 40); // left iris
    fill(white);
    circle(72, 40, 40); // right iris
    fill(white);
    circle(-40, 20, 20); // left eyeshine
    fill(white);
    circle(104, 20, 20); // right eyeshine
    fill(black);
    circle(0, 120, 8); // mouth
  }
}

void addSubtleBee(float x, float y) {
  translate(x, y);
  if (emoteJ) {                                              
    noStroke();                                                    
    fill(120, 250, 255);
    circle(68, 76, 160); //right wing
    fill(120, 250, 255);
    circle(-68, 76, 160); //left wing
    fill(205, 175, 250);
    circle(0, 24, beeWidth); // bee's body
    fill(black);
    ellipse(-72, 10, 120, 10); // left eye
    fill(black);
    ellipse(72, 10, 120, 10); // right eye
    fill(255, 150, 190);
    ellipse(-72, 40, 80, 40); // left blush
    fill(255, 150, 190);
    ellipse(72, 40, 80, 40); // right blush
  } else if (emoteI) {
    noStroke();
    fill(120, 250, 255);
    circle(68, 70, 160); //right wing
    fill(120, 250, 255);
    circle(-68, 70, 160); //left wing
    fill(205, 175, 250);
    circle(0, 40, beeWidth); // bee's body
    fill(black);
    ellipse(-62, 70, 100, 10); // left eye
    fill(black);
    ellipse(62, 70, 100, 10); // right eye
    fill(black);
    circle(0, 90, 20);
  } else if (emoteH) {
    noStroke();
    fill(120, 250, 255);
    circle(68, 40, 160); //right wing
    fill(120, 250, 255);
    circle(-68, 40, 160); //left wing
    fill(205, 175, 250);
    circle(0, 40, beeWidth); // bee's body
    fill(black);
    ellipse(-72, 70, 10, 10); // left eye
    fill(black);
    ellipse(72, 70, 10, 10); // right eye
  } else if (emoteG) {
    noStroke();
    fill(120, 250, 255);
    circle(68, 70, 160); //right wing
    fill(120, 250, 255);
    circle(-68, 70, 160); //left wing
    fill(205, 175, 250);
    circle(0, 40, beeWidth); // bee's body
    fill(black);
    ellipse(-72, 0, 130, 10); // left eye
    fill(black);
    ellipse(72, 0, 130, 10); // right eye
  } else if (emoteF) {
    noStroke();
    fill(120, 250, 255);
    circle(68, 50, 160); //right wing
    fill(120, 250, 255);
    circle(-68, 50, 160); //left wing
    fill(205, 175, 250);
    circle(0, 40, beeWidth); // bee's body
    fill(black);
    ellipse(-72, 80, 100, 50); // left eye
    fill(black);
    ellipse(72, 80, 100, 50); // right eye
  } else if (emoteE) {
    noStroke();
    fill(120, 250, 255);
    circle(58, 70, 160); //right wing
    fill(120, 250, 255);
    circle(-58, 70, 160); //left wing
    fill(205, 175, 250);
    circle(0, 40, beeWidth); // bee's body
    fill(black);
    ellipse(-42, -40, 70, 10); // left eye
    fill(black);
    ellipse(42, -40, 70, 10); // right eye
  } else if (emoteD) {
    noStroke();
    fill(120, 250, 255);
    circle(68, 50, 160); //right wing
    fill(120, 250, 255);
    circle(-68, 60, 160); //left wing
    fill(205, 175, 250);
    circle(0, 40, beeWidth); // bee's body
    fill(100, 150, 255);
    ellipse(-72, 110, 50, 15); // left tear
    fill(100, 150, 255);
    ellipse(72, 110, 50, 15); // right tear
    fill(black);
    ellipse(-62, 100, 90, 10); // left eye
    fill(black);
    ellipse(62, 100, 90, 10); // right eye
  } else if (emoteC) {
    noStroke();
    fill(120, 250, 255);
    circle(78, -7, 160); //right wing
    fill(120, 250, 255);
    circle(-78, -17, 160); //left wing
    fill(205, 175, 250);
    circle(0, 40, beeWidth); // bee's body
    fill(black);
    ellipse(-72, 70, 120, 10); // left eye
    fill(black);
    ellipse(72, 80, 120, 10); // right eye
  } else if (emoteB) {
    noStroke();
    fill(120, 250, 255);
    circle(68, 70, 160); //right wing
    fill(120, 250, 255);
    circle(-68, 70, 160); //left wing
    fill(205, 175, 250);
    circle(0, 40, beeWidth); // bee's body
    fill(black);
    ellipse(-72, 90, 120, 10); // left eye
    fill(black);
    ellipse(72, 90, 120, 10); // right eye
  } else if (emoteA) {
    noStroke();
    fill(120, 250, 255);
    circle(68, 70, 160); //right wing
    fill(120, 250, 255);
    circle(-68, 70, 160); //left wing
    fill(205, 175, 250);
    circle(0, 40, beeWidth); // bee's body
    fill(black);
    ellipse(-72, 70, 120, 10); // left eye
    fill(black);
    ellipse(72, 70, 120, 10); // right eye
  }
}
