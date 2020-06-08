// BSc Creative Computing
// Unit: Sound and Image Processing
// Sketch 2: Game of Life Simulation
// Apart of the "Build a Turnip" series. This assignment is a simulation of Cornwall's game of life. This assignment utilize the nested conditionals methods taught in class. It also utilise different class functions for Cornwall's game of life rules, population and generation counter, and user instructions. 
// when the population is stale or when the population dies out, there will be a pop up that tells the user the condition. 

// Instruction: Click on the "regenerate" button to start a new generation of turnips. 


//image variables
let border;
let turnip;
let extinct;
let stale;
let regen;
let ffont

//variable for instruction button
a = 0;
let click;
let inst_array = ["filler.png", "condition.png"];
let con;

//screen detail variables
const screen_size = 1000,
  icon_size = 50,
  elements_ = screen_size / icon_size;

//class object variables
var main_screen;
var new_screen;
var population;
var generation;
var last_turnip_x;
var last_turnip_y;
var screen_detail;
var initial_;
var timer;

function preload() {
  border = loadImage("border1.png");
  turnip = loadImage("turnip.png");
  ffont = loadFont('game_over.ttf');
  extinct = loadImage("extinct.png");
  stale = loadImage("stop.png");
  regen = loadImage("regenerate.png")
  con = loadImage("condition1.png")
  click = loadSound("Clicking-sound-effect.mp3");
  condition = loadImage(inst_array[a]);
}

function setup() {
  createCanvas(1200, 1200);
  createArrays();
  initial_var(true); //start simulation
  image(border, 0, 0, width, height); //border of simulation

}

function draw() {
  //starting simulation condition
  if (!initial_) {
    if (timer == 4.5) {
      gol_conditions();
      new_grid();
      population_counter();
      screen_turnips();
      detail_screen_();
      
      generation++;
      timer = 0;
    }
    timer += 0.5;
  } else {
    population_counter();
    screen_turnips();
    detail_screen_();
  }

}

function createArrays() {
  main_screen = new Array(elements_);
  new_screen = new Array(elements_);

  for (var i = 0; i < elements_; i++) {
    main_screen[i] = new Array(elements_);
    new_screen[i] = new Array(elements_);
  }
}

function initial_var(flag) {
  var binaryValuesArray = [1, 0, 0, 0, 0, 0, 0, 0, 0, 0];

  for (var i = 0; i < elements_; i++) {
    for (var j = 0; j < elements_; j++) {
      main_screen[i][j] = random(binaryValuesArray);
      new_screen[i][j] = main_screen[i][j];
    }
  }

  generation = 0;
  screen_detail = flag;
  initial_ = false;
  last_turnip_x = -1;
  last_turnip_y = -1;
  population = 0;
  timer = 4.5;
}

function screen_turnips() {
  noStroke();

  fill(139, 203, 210); //background
  rect(100, 100, screen_size, screen_size);
  image(regen, 0, 0, width, height);

  for (var y = 150, i = 0; y < 1050; y += icon_size, i++) {
    for (var x = 150, j = 0; x < 1050; x += icon_size, j++) {
      if (main_screen[i][j]) image(turnip, x, y, icon_size, icon_size);
    }
  }
}
//}

function detail_screen_() {
  textFont(ffont);
  noStroke();

  //border for text or button detail
  fill(139, 203, 210);
  rect(850, 25, 320, 55);

  fill(220, 119, 158);
  rect(30, 25, 190, 55)

  textSize(55)
  fill(44, 80, 84);
  text("Population: " + population, 860, 60);
  text("Generation: " + generation, 1015, 60);

  textSize(65);
  fill(125, 47, 77);
  text("Instruction", 55, 60);


  //condition if population dies 
  if (population < 1) {
    image(extinct, 0, 0, width, height);
  }

  //condition if population is stale
  if (population < 11) {
    if (population > 1) {
      image(stale, 0, 0, width, height);
    }
  }

  //insturction image array. pop up when user click this button. 
  if (a == 0) {

  } else if (a == 1) {
    image(con, 0, 0, width, height);
  }

}


function emptyGrid() {
  generation = 0;

  for (var i = 0; i < elements_; i++) {
    for (var j = 0; j < elements_; j++) {
      new_screen[i][j] = 0;
    }
  }
}

function gol_conditions() {
  //condition function for center, corner and edges
  
  for (var i = 0; i < elements_; i++) {
    for (var j = 0; j < elements_; j++) {
      var turnip = 0

      // Corners condition
      if (i == 0 && j == 0) {
        if (main_screen[i][j + 1]) turnip++;
        if (main_screen[i + 1][j]) turnip++;
        if (main_screen[i + 1][j + 1]) turnip++;
      } else if (i == 0 && j == (elements_ - 1)) {
        if (main_screen[i][j - 1]) turnip++;
        if (main_screen[i + 1][j]) turnip++;
        if (main_screen[i + 1][j - 1]) turnip++;
      } else if (i == (elements_ - 1) && j == 0) {
        if (main_screen[i][j + 1]) turnip++;
        if (main_screen[i - 1][j]) turnip++;
        if (main_screen[i - 1][j + 1]) turnip++;
      } else if (i == (elements_ - 1) && j == (elements_ - 1)) {
        if (main_screen[i][j - 1]) turnip++;
        if (main_screen[i - 1][j]) turnip++;
        if (main_screen[i - 1][j - 1]) turnip++;
      }
      // Border conditions
      else if (i == 0 && (j > 0 && j < (elements_ - 1))) {
        if (main_screen[i][j - 1]) turnip++;
        if (main_screen[i][j + 1]) turnip++;
        if (main_screen[i + 1][j - 1]) turnip++;
        if (main_screen[i + 1][j]) turnip++;
        if (main_screen[i + 1][j + 1]) turnip++;
      } else if (i == (elements_ - 1) && (j > 0 && j < (elements_ - 1))) {
        if (main_screen[i][j - 1]) turnip++;
        if (main_screen[i][j + 1]) turnip++;
        if (main_screen[i - 1][j - 1]) turnip++;
        if (main_screen[i - 1][j]) turnip++;
        if (main_screen[i - 1][j + 1]) turnip++;
      } else if ((i > 0 && i < (elements_ - 1)) && j == 0) {
        if (main_screen[i - 1][j]) turnip++;
        if (main_screen[i + 1][j]) turnip++;
        if (main_screen[i - 1][j + 1]) turnip++;
        if (main_screen[i][j + 1]) turnip++;
        if (main_screen[i + 1][j + 1]) turnip++;
      } else if ((i > 0 && i < (elements_ - 1)) && j == (elements_ - 1)) {
        if (main_screen[i - 1][j]) turnip++;
        if (main_screen[i + 1][j]) turnip++;
        if (main_screen[i - 1][j - 1]) turnip++;
        if (main_screen[i][j - 1]) turnip++;
        if (main_screen[i + 1][j - 1]) turnip++;
      }
      // center/general condition
      else {
        if (main_screen[i - 1][j - 1]) turnip++;
        if (main_screen[i - 1][j]) turnip++;
        if (main_screen[i - 1][j + 1]) turnip++;
        if (main_screen[i][j - 1]) turnip++;
        if (main_screen[i][j + 1]) turnip++;
        if (main_screen[i + 1][j - 1]) turnip++;
        if (main_screen[i + 1][j]) turnip++;
        if (main_screen[i + 1][j + 1]) turnip++;
      }

      // Applying changes to a secondary array.
      if (main_screen[i][j]) {
        if (turnip < 2) new_screen[i][j] = 0;
        else if (turnip > 3) new_screen[i][j] = 0;
      } else {
        if (turnip == 3) new_screen[i][j] = 1;
      }
    }
  }
}

function new_grid() {
  for (var i = 0; i < elements_; i++) {
    for (var j = 0; j < elements_; j++) {
      main_screen[i][j] = new_screen[i][j];
    }
  }
}

function population_counter() {
  population = 0;
  for (var i = 0; i < elements_; i++) {
    for (var j = 0; j < elements_; j++) {
      if (main_screen[i][j]) population++;
    }
  }
}

function mousePressed() {

  //let user restart generation
  let screen_dist = dist(mouseX, mouseY, 600, 1100);
  if (screen_dist < 90) {
    click.play();
    initial_var(screen_detail);
  }


  //instruction pop up
  if (a >= 1) {
    a = -1;
  }

  let inst_dist = dist(mouseX, mouseY, 30, 25);
  if (inst_dist < 200) {
    a++
    click.play();
    condition = loadImage(inst_array[a]);
  }

}
