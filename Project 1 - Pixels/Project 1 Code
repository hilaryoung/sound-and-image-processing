// BSc Creative Computing
// Unit: Sound and Image Processing
// Sketch 1: Build a Turnip 
// "Build a Turnip" is a mini dress up game utilising pixels to process images. Specifically I use the basic understanding of creating a mosaic filter, however I made the windowSize 6 pixels, in order to mantain the form of the images. I also add in a "save" button to save the User's designed turnip. 
// Instruction: Click on the arrow button to change the apperance of the turnip, press the save when done.

// Set variables
// the " letter = 0; " is a counter that corresponds to the mousePress() function 

var backg;
var click_s;
var save_button;
var logo;
var back_sound;

//body
var body1;   var body2;   var body3;   var body4;
let a = 0;

//head
var head1;   var head2;   var head3;   var head4;
let b = 0;

//eyes
var eyes1;   var eyes2;   var eyes3;   var eyes4;   
let c = 0;

//mouth
var mouth1;   var mouth2;   var mouth3;   var mouth4;
let d = 0;

//accesory
var ac1;   var ac2;   var ac3;   var ac4;
let e = 0;

//landscape
var land1;   var land2;   var land3;   var land4;
var land5;   var land6;   var land7;   var land8;
var land9;   var land10;  var land11;  var land12;
var land13;  var land14;  var land15;  var land16;
f = 0;

function preload() {

  backg = loadImage("background.png");
  click_s = loadSound("Clicking-sound-effect.mp3");
  save_button = loadImage("save button.png");
  logo = loadImage("logo.png");
  back_sound = createAudio("tune.mp3");

  //body
  body1 = loadImage("body1.png");    body2 = loadImage("body2.png");
  body3 = loadImage("body3.png");    body4 = loadImage("body4.png");

  //head
  head1 = loadImage("head1.png");    head2 = loadImage("head2.png");
  head3 = loadImage("head3.png");    head4 = loadImage("head4.png");

  //eyes
  eyes1 = loadImage("eyes1.png");    eyes2 = loadImage("eyes2.png");
  eyes3 = loadImage("eyes3.png");    eyes4 = loadImage("eyes4.png");

  //mouth
  mouth1 = loadImage("mouth1.png");    mouth2 = loadImage("mouth2.png");
  mouth3 = loadImage("mouth3.png");    mouth4 = loadImage("mouth4.png");

  //accesory
  ac1 = loadImage("ac1.png");    ac2 = loadImage("ac2.png");
  ac3 = loadImage("ac3.png");    ac4 = loadImage("ac4.png");

  //landscape
  land1 = loadImage("land1.png");    land2 = loadImage("land2.png");    land3 = loadImage("land3.png");
  land4 = loadImage("land4.png");    land5 = loadImage("land5.png");    land6 = loadImage("land6.png");
  land7 = loadImage("land7.png");    land8 = loadImage("land8.png");    land9 = loadImage("land9.png");
  land10 = loadImage("land10.png");  land11 = loadImage("land11.png");  land12 = loadImage("land12.png");
  land13 = loadImage("land13.png");  land14 = loadImage("land14.png");  land15 = loadImage("land15.png");
  land16 = loadImage("land16.png");
}

function setup() {
  createCanvas(1400, 1000);
  noStroke();
  back_sound.volume(0.35);
  back_sound.loop();
  back_sound.play();
}

function draw() {
  //window size for the pixels
  const window_size = 6;
  //landscape///////////////////////////////////////////////////////////////////////////////////////
  if (f == 0) {
    land1.loadPixels(); //load pixels
    for (let y = 0; y < land1.height; y += window_size) {
      for (let x = 0; x < land1.width; x += window_size) {
        const pixValue = (y * land1.width + x) * 4; // change final multiplier for pixel squares
        const colR = (land1.pixels[pixValue]);
        const colG = (land1.pixels[pixValue + 1]);
        const colB = (land1.pixels[pixValue + 2]);
        const colA = (land1.pixels[pixValue + 3]);
        fill(colR, colG, colB, colA);
        rect(x, y, window_size, window_size);
      }
    }
  } else if (f == 1) {
    land2.loadPixels();
    for (let y = 0; y < land2.height; y += window_size) {
      for (let x = 0; x < land2.width; x += window_size) {
        const pixValue = (y * land2.width + x) * 4;
        const colR = (land2.pixels[pixValue]);
        const colG = (land2.pixels[pixValue + 1]);
        const colB = (land2.pixels[pixValue + 2]);
        const colA = (land2.pixels[pixValue + 3]);

        fill(colR, colG, colB, colA);
        rect(x, y, window_size, window_size);
      }
    }
  } else if (f == 2) {
    land3.loadPixels();
    for (let y = 0; y < land3.height; y += window_size) {
      for (let x = 0; x < land3.width; x += window_size) {
        const pixValue = (y * land3.width + x) * 4;
        const colR = (land3.pixels[pixValue]);
        const colG = (land3.pixels[pixValue + 1]);
        const colB = (land3.pixels[pixValue + 2]);
        const colA = (land3.pixels[pixValue + 3]);
        fill(colR, colG, colB, colA);
        rect(x, y, window_size, window_size);
      }
    }
  } else if (f == 3) {
    land4.loadPixels();
    for (let y = 0; y < land4.height; y += window_size) {
      for (let x = 0; x < land4.width; x += window_size) {
        const pixValue = (y * land4.width + x) * 4;
        const colR = (land4.pixels[pixValue]);
        const colG = (land4.pixels[pixValue + 1]);
        const colB = (land4.pixels[pixValue + 2]);
        const colA = (land4.pixels[pixValue + 3]);
        fill(colR, colG, colB, colA);
        rect(x, y, window_size, window_size);
      }
    }
  } else if (f == 4) {
    land5.loadPixels();
    for (let y = 0; y < land5.height; y += window_size) {
      for (let x = 0; x < land5.width; x += window_size) {
        const pixValue = (y * land5.width + x) * 4;
        const colR = (land5.pixels[pixValue]);
        const colG = (land5.pixels[pixValue + 1]);
        const colB = (land5.pixels[pixValue + 2]);
        const colA = (land5.pixels[pixValue + 3]);
        fill(colR, colG, colB, colA);
        rect(x, y, window_size, window_size);
      }
    }
  } else if (f == 5) {
    land6.loadPixels();
    for (let y = 0; y < land6.height; y += window_size) {
      for (let x = 0; x < land6.width; x += window_size) {
        const pixValue = (y * land6.width + x) * 4;
        const colR = (land6.pixels[pixValue]);
        const colG = (land6.pixels[pixValue + 1]);
        const colB = (land6.pixels[pixValue + 2]);
        const colA = (land6.pixels[pixValue + 3]);
        fill(colR, colG, colB, colA);
        rect(x, y, window_size, window_size);
      }
    }
  } else if (f == 6) {
    land7.loadPixels();
    for (let y = 0; y < land7.height; y += window_size) {
      for (let x = 0; x < land7.width; x += window_size) {
        const pixValue = (y * land7.width + x) * 4;
        const colR = (land7.pixels[pixValue]);
        const colG = (land7.pixels[pixValue + 1]);
        const colB = (land7.pixels[pixValue + 2]);
        const colA = (land7.pixels[pixValue + 3]);
        fill(colR, colG, colB, colA);
        rect(x, y, window_size, window_size);
      }
    }
  } else if (f == 7) {
    land8.loadPixels();
    for (let y = 0; y < land8.height; y += window_size) {
      for (let x = 0; x < land8.width; x += window_size) {
        const pixValue = (y * land8.width + x) * 4;
        const colR = (land8.pixels[pixValue]);
        const colG = (land8.pixels[pixValue + 1]);
        const colB = (land8.pixels[pixValue + 2]);
        const colA = (land8.pixels[pixValue + 3]);
        fill(colR, colG, colB, colA);
        rect(x, y, window_size, window_size);
      }
    }
  } else if (f == 8) {
    land9.loadPixels();
    for (let y = 0; y < land9.height; y += window_size) {
      for (let x = 0; x < land9.width; x += window_size) {
        const pixValue = (y * land9.width + x) * 4;
        const colR = (land9.pixels[pixValue]);
        const colG = (land9.pixels[pixValue + 1]);
        const colB = (land9.pixels[pixValue + 2]);
        const colA = (land9.pixels[pixValue + 3]);
        fill(colR, colG, colB, colA);
        rect(x, y, window_size, window_size);
      }
    }
  } else if (f == 9) {
    land10.loadPixels();
    for (let y = 0; y < land10.height; y += window_size) {
      for (let x = 0; x < land10.width; x += window_size) {
        const pixValue = (y * land10.width + x) * 4;
        const colR = (land10.pixels[pixValue]);
        const colG = (land10.pixels[pixValue + 1]);
        const colB = (land10.pixels[pixValue + 2]);
        const colA = (land10.pixels[pixValue + 3]);
        fill(colR, colG, colB, colA);
        rect(x, y, window_size, window_size);
      }
    }
  } else if (f == 10) {
    land11.loadPixels();
    for (let y = 0; y < land11.height; y += window_size) {
      for (let x = 0; x < land11.width; x += window_size) {
        const pixValue = (y * land11.width + x) * 4;
        const colR = (land11.pixels[pixValue]);
        const colG = (land11.pixels[pixValue + 1]);
        const colB = (land11.pixels[pixValue + 2]);
        const colA = (land11.pixels[pixValue + 3]);
        fill(colR, colG, colB, colA);
        rect(x, y, window_size, window_size);
      }
    }
  } else if (f == 11) {
    land12.loadPixels();
    for (let y = 0; y < land12.height; y += window_size) {
      for (let x = 0; x < land12.width; x += window_size) {
        const pixValue = (y * land12.width + x) * 4;
        const colR = (land12.pixels[pixValue]);
        const colG = (land12.pixels[pixValue + 1]);
        const colB = (land12.pixels[pixValue + 2]);
        const colA = (land12.pixels[pixValue + 3]);
        fill(colR, colG, colB, colA);
        rect(x, y, window_size, window_size);
      }
    }
  } else if (f == 12) {
    land13.loadPixels();
    for (let y = 0; y < land13.height; y += window_size) {
      for (let x = 0; x < land13.width; x += window_size) {
        const pixValue = (y * land13.width + x) * 4;
        const colR = (land13.pixels[pixValue]);
        const colG = (land13.pixels[pixValue + 1]);
        const colB = (land13.pixels[pixValue + 2]);
        const colA = (land13.pixels[pixValue + 3]);
        fill(colR, colG, colB, colA);
        rect(x, y, window_size, window_size);
      }
    }
  } else if (f == 13) {
    land14.loadPixels();
    for (let y = 0; y < land14.height; y += window_size) {
      for (let x = 0; x < land14.width; x += window_size) {
        const pixValue = (y * land14.width + x) * 4;
        const colR = (land14.pixels[pixValue]);
        const colG = (land14.pixels[pixValue + 1]);
        const colB = (land14.pixels[pixValue + 2]);
        const colA = (land14.pixels[pixValue + 3]);
        fill(colR, colG, colB, colA);
        rect(x, y, window_size, window_size);
      }
    }
  } else if (f == 14) {
    land15.loadPixels();

    for (let y = 0; y < land15.height; y += window_size) {
      for (let x = 0; x < land15.width; x += window_size) {
        const pixValue = (y * land15.width + x) * 4;
        const colR = (land15.pixels[pixValue]);
        const colG = (land15.pixels[pixValue + 1]);
        const colB = (land15.pixels[pixValue + 2]);
        const colA = (land15.pixels[pixValue + 3]);
        fill(colR, colG, colB, colA);
        rect(x, y, window_size, window_size);
      }
    }
  } else if (f == 15) {
    land16.loadPixels();
    for (let y = 0; y < land16.height; y += window_size) {
      for (let x = 0; x < land16.width; x += window_size) {
        const pixValue = (y * land16.width + x) * 4;
        const colR = (land16.pixels[pixValue]);
        const colG = (land16.pixels[pixValue + 1]);
        const colB = (land16.pixels[pixValue + 2]);
        const colA = (land16.pixels[pixValue + 3]);
        fill(colR, colG, colB, colA);
        rect(x, y, window_size, window_size);
      }
    }
  }
  //head ///////////////////////////////////////////////////////////////////////////////////////
  if (b == 0) {
    head1.loadPixels();
    for (let y = 0; y < head1.height; y += window_size) {
      for (let x = 0; x < head1.width; x += window_size) {
        const pixValue = (y * head1.width + x) * 4;
        const colR = (head1.pixels[pixValue]);
        const colG = (head1.pixels[pixValue + 1]);
        const colB = (head1.pixels[pixValue + 2]);
        const colA = (head1.pixels[pixValue + 3]);
        fill(colR, colG, colB, colA);
        rect(x, y, window_size, window_size);
      }
    }
  } else if (b == 1) {
    head2.loadPixels();
    for (let y = 0; y < head2.height; y += window_size) {
      for (let x = 0; x < head2.width; x += window_size) {
        const pixValue = (y * head2.width + x) * 4;
        const colR = (head2.pixels[pixValue]);
        const colG = (head2.pixels[pixValue + 1]);
        const colB = (head2.pixels[pixValue + 2]);
        const colA = (head2.pixels[pixValue + 3]);
        fill(colR, colG, colB, colA);
        rect(x, y, window_size, window_size);
      }
    }
  } else if (b == 2) {
    head3.loadPixels();
    for (let y = 0; y < head3.height; y += window_size) {
      for (let x = 0; x < head3.width; x += window_size) {
        const pixValue = (y * head3.width + x) * 4;
        const colR = (head3.pixels[pixValue]);
        const colG = (head3.pixels[pixValue + 1]);
        const colB = (head3.pixels[pixValue + 2]);
        const colA = (head3.pixels[pixValue + 3]);
        fill(colR, colG, colB, colA);
        rect(x, y, window_size, window_size);
      }
    }
  } else if (b == 3) {
    head4.loadPixels();

    for (let y = 0; y < head4.height; y += window_size) {
      for (let x = 0; x < head4.width; x += window_size) {
        const pixValue = (y * head4.width + x) * 4;
        const colR = (head4.pixels[pixValue]);
        const colG = (head4.pixels[pixValue + 1]);
        const colB = (head4.pixels[pixValue + 2]);
        const colA = (head4.pixels[pixValue + 3]);
        fill(colR, colG, colB, colA);
        rect(x, y, window_size, window_size);
      }
    }
  }
  //body ///////////////////////////////////////////////////////////////////////////////////////
  if (a == 0) {
    body1.loadPixels();
    for (let y = 0; y < body1.height; y +=window_size) {
      for (let x = 0; x < body1.width; x +=window_size) {
        const pixValue = (y * body1.width + x) * 4;
        const colR = (body1.pixels[pixValue]);
        const colG = (body1.pixels[pixValue + 1]);
        const colB = (body1.pixels[pixValue + 2]);
        const colA = (body1.pixels[pixValue + 3]);
        fill(colR, colG, colB, colA);
        rect(x, y,window_size,window_size);
      }
    }
  } else if (a == 1) {
    body2.loadPixels();
    for (let y = 0; y < body2.height; y +=window_size) {
      for (let x = 0; x < body2.width; x +=window_size) {
        const pixValue = (y * body2.width + x) * 4;
        const colR = (body2.pixels[pixValue]);
        const colG = (body2.pixels[pixValue + 1]);
        const colB = (body2.pixels[pixValue + 2]);
        const colA = (body2.pixels[pixValue + 3]);
        fill(colR, colG, colB, colA);
        rect(x, y,window_size,window_size);
      }
    }
  } else if (a == 2) {
    body3.loadPixels();
    for (let y = 0; y < body3.height; y +=window_size) {
      for (let x = 0; x < body3.width; x +=window_size) {
        const pixValue = (y * body3.width + x) * 4;
        const colR = (body3.pixels[pixValue]);
        const colG = (body3.pixels[pixValue + 1]);
        const colB = (body3.pixels[pixValue + 2]);
        const colA = (body3.pixels[pixValue + 3]);
        fill(colR, colG, colB, colA);
        rect(x, y,window_size,window_size);
      }
    }
  } else if (a == 3) {
    body4.loadPixels();
    for (let y = 0; y < body4.height; y +=window_size) {
      for (let x = 0; x < body4.width; x +=window_size) {
        const pixValue = (y * body4.width + x) * 4;
        const colR = (body4.pixels[pixValue]);
        const colG = (body4.pixels[pixValue + 1]);
        const colB = (body4.pixels[pixValue + 2]);
        const colA = (body4.pixels[pixValue + 3]);
        fill(colR, colG, colB, colA);
        rect(x, y,window_size,window_size);
      }
    }
  }
  //eyes ///////////////////////////////////////////////////////////////////////////////////////
  if (c == 0) {
    eyes1.loadPixels();

    for (let y = 0; y < eyes1.height; y += window_size) {
      for (let x = 0; x < eyes1.width; x += window_size) {
        const pixValue = (y * eyes1.width + x) * 4;
        const colR = (eyes1.pixels[pixValue]);
        const colG = (eyes1.pixels[pixValue + 1]);
        const colB = (eyes1.pixels[pixValue + 2]);
        const colA = (eyes1.pixels[pixValue + 3]);
        fill(colR, colG, colB, colA);
        rect(x, y, window_size, window_size);
      }
    }
  } else if (c == 1) {
    eyes2.loadPixels();
    for (let y = 0; y < eyes2.height; y += window_size) {
      for (let x = 0; x < eyes2.width; x += window_size) {
        const pixValue = (y * eyes2.width + x) * 4;
        const colR = (eyes2.pixels[pixValue]);
        const colG = (eyes2.pixels[pixValue + 1]);
        const colB = (eyes2.pixels[pixValue + 2]);
        const colA = (eyes2.pixels[pixValue + 3]);
        fill(colR, colG, colB, colA);
        rect(x, y, window_size, window_size);
      }
    }
  } else if (c == 2) {
    eyes3.loadPixels();
    for (let y = 0; y < eyes3.height; y += window_size) {
      for (let x = 0; x < eyes3.width; x += window_size) {
        const pixValue = (y * eyes3.width + x) * 4;
        const colR = (eyes3.pixels[pixValue]);
        const colG = (eyes3.pixels[pixValue + 1]);
        const colB = (eyes3.pixels[pixValue + 2]);
        const colA = (eyes3.pixels[pixValue + 3]);
        fill(colR, colG, colB, colA);
        rect(x, y, window_size, window_size);
      }
    }
  } else if (c == 3) {
    eyes4.loadPixels();
    for (let y = 0; y < eyes4.height; y += window_size) {
      for (let x = 0; x < eyes4.width; x += window_size) {
        const pixValue = (y * eyes4.width + x) * 4;
        const colR = (eyes4.pixels[pixValue]);
        const colG = (eyes4.pixels[pixValue + 1]);
        const colB = (eyes4.pixels[pixValue + 2]);
        const colA = (eyes4.pixels[pixValue + 3]);
        fill(colR, colG, colB, colA);
        rect(x, y, window_size, window_size);
      }
    }
  }
  //mouth ///////////////////////////////////////////////////////////////////////////////////////
  if (d == 0) {
    mouth1.loadPixels();
    for (let y = 0; y < mouth1.height; y += window_size) {
      for (let x = 0; x < mouth1.width; x += window_size) {
        const pixValue = (y * mouth1.width + x) * 4;
        const colR = (mouth1.pixels[pixValue]);
        const colG = (mouth1.pixels[pixValue + 1]);
        const colB = (mouth1.pixels[pixValue + 2]);
        const colA = (mouth1.pixels[pixValue + 3]);
        fill(colR, colG, colB, colA);
        rect(x, y, window_size, window_size);
      }
    }
  } else if (d == 1) {
    mouth2.loadPixels();
    for (let y = 0; y < mouth2.height; y += window_size) {
      for (let x = 0; x < mouth2.width; x += window_size) {
        const pixValue = (y * mouth2.width + x) * 4;
        const colR = (mouth2.pixels[pixValue]);
        const colG = (mouth2.pixels[pixValue + 1]);
        const colB = (mouth2.pixels[pixValue + 2]);
        const colA = (mouth2.pixels[pixValue + 3]);
        fill(colR, colG, colB, colA);
        rect(x, y, window_size, window_size);
      }
    }
  } else if (d == 2) {
    mouth3.loadPixels();
    for (let y = 0; y < mouth3.height; y += window_size) {
      for (let x = 0; x < mouth3.width; x += window_size) {
        const pixValue = (y * mouth3.width + x) * 4;
        const colR = (mouth3.pixels[pixValue]);
        const colG = (mouth3.pixels[pixValue + 1]);
        const colB = (mouth3.pixels[pixValue + 2]);
        const colA = (mouth3.pixels[pixValue + 3]);
        fill(colR, colG, colB, colA);
        rect(x, y, window_size, window_size);
      }
    }
  } else if (d == 3) {
    mouth4.loadPixels();
    for (let y = 0; y < mouth4.height; y += window_size) {
      for (let x = 0; x < mouth4.width; x += window_size) {
        const pixValue = (y * mouth4.width + x) * 4;
        const colR = (mouth4.pixels[pixValue]);
        const colG = (mouth4.pixels[pixValue + 1]);
        const colB = (mouth4.pixels[pixValue + 2]);
        const colA = (mouth4.pixels[pixValue + 3]);
        fill(colR, colG, colB, colA);
        rect(x, y, window_size, window_size);
      }
    }
  }
  //accesory ///////////////////////////////////////////////////////////////////////////////////////
  if (e == 0) {
    ac1.loadPixels();
    //nothing
  } else if (e == 1) {
    ac2.loadPixels();
    for (let y = 0; y < ac2.height; y += window_size) {
      for (let x = 0; x < ac2.width; x += window_size) {
        const pixValue = (y * ac2.width + x) * 4;
        const colR = (ac2.pixels[pixValue]);
        const colG = (ac2.pixels[pixValue + 1]);
        const colB = (ac2.pixels[pixValue + 2]);
        const colA = (ac2.pixels[pixValue + 3]);
        fill(colR, colG, colB, colA);
        rect(x, y, window_size, window_size);
      }
    }
  } else if (e == 2) {
    ac3.loadPixels();
    for (let y = 0; y < ac3.height; y += window_size) {
      for (let x = 0; x < ac3.width; x += window_size) {
        const pixValue = (y * ac3.width + x) * 4;
        const colR = (ac3.pixels[pixValue]);
        const colG = (ac3.pixels[pixValue + 1]);
        const colB = (ac3.pixels[pixValue + 2]);
        const colA = (ac3.pixels[pixValue + 3]);
        fill(colR, colG, colB, colA);
        rect(x, y, window_size, window_size);
      }
    }
  } else if (e == 3) {
    ac4.loadPixels();
    for (let y = 0; y < ac4.height; y += window_size) {
      for (let x = 0; x < ac4.width; x += window_size) {
        const pixValue = (y * ac4.width + x) * 4;
        const colR = (ac4.pixels[pixValue]);
        const colG = (ac4.pixels[pixValue + 1]);
        const colB = (ac4.pixels[pixValue + 2]);
        const colA = (ac4.pixels[pixValue + 3]);
        fill(colR, colG, colB, colA);
        rect(x, y, window_size, window_size);
      }
    }
  } else if (e == 4) {
    ac1.loadPixels();
    for (let y = 0; y < ac1.height; y += window_size) {
      for (let x = 0; x < ac1.width; x += window_size) {
        const pixValue = (y * ac1.width + x) * 4;
        const colR = (ac1.pixels[pixValue]);
        const colG = (ac1.pixels[pixValue + 1]);
        const colB = (ac1.pixels[pixValue + 2]);
        const colA = (ac1.pixels[pixValue + 3]);
        fill(colR, colG, colB, colA);
        rect(x, y, window_size, window_size);
      }
    }
  }
  image(backg, 0, 0, width, height);
  image(save_button, 830, 820, 90, 90);
  image(logo,967,80,290,290);
  
}
function mousePressed() {
  //body
  if (a >= 3) {
    a = -1;
  } let k = dist(mouseX, mouseY, 1185, 370);
  if (k < 40) {
    a++;
    click_s.play();
  }
  //head
  if (b >= 3) {
    b = -1;
  } let l = dist(mouseX, mouseY, 1185, 460);
  if (l < 40) {
    b++;
    click_s.play();
  }
  //eyes
  if (c >= 3) {
    c = -1;
  } let m = dist(mouseX, mouseY, 1185, 550);
  if (m < 40) {
    c++;
    click_s.play();
  }
  //mouth
  if (d >= 3) {
    d = -1;
  } let n = dist(mouseX, mouseY, 1185, 640);
  if (n < 40) {
    d++;
    click_s.play();
  }
  //accesory
  if (e >= 4) {
    e = -1;
  } let o = dist(mouseX, mouseY, 1185, 730);
  if (o < 40) {
    e++;
    click_s.play();
  }
  //landscape
  if (f >= 16) {
    f = -1;
  } let p = dist(mouseX, mouseY, 1185, 840);
  if (p < 40) {
    f++;
    click_s.play();
  }
  //save button
  let save_dist = dist(mouseX, mouseY, 830, 820);
  if (save_dist < 80) {
    click_s.play();
    let to_save = get(260, 210, 565, 590);
    to_save.save("your turnip.png");
  }
}
