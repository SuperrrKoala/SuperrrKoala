//Assignment#12_Ziyi Long

void setup()
{
  size(800,900);
}

// Here is my background!

void draw(){
  background(255,103,142);
  noStroke();

  fill(255,216,57);
  rect(0,360,800,80);
  
  fill(187,255,111);
  rect(0,440,800,550);
  
  fill(111,189,255);
  rect(0,520,800,550);
 
  noStroke();

// Here is the first part of my hair
  fill(0);
  rect(170,380,460,320);
  triangle(200,380,200,700,150,700);
  triangle(200,380,200,700,150,700);
  
//Here are the two ears
  fill(255,232,222); 
  ellipse(200,480, 80,100);
  ellipse(600,480, 80,100);
 
//Face
  fill(255,232,222); 
  ellipse(400,445, 400,450);
  
//Neck
  rect(360,530,80,180);

//Nose  
  fill(255,195,161);
  triangle(400,450,425,540,375,540);
  
//Mouth
  stroke(255,113,113);
  line(350, 585, 450, 585);
  
 //Here are the bangs
  noStroke();
  fill(0);
  arc(400,390,460,450, radians(180), radians(360));
  
 //forehead
  fill(255,232,222); 
  triangle(450,290, 208,390, 595, 390);
  
 // eyelash
  stroke(0);
  strokeWeight(10);
  line(270,390,300,440);
  line(250,400,300,440);
  line(235,415,300,440);
  line(530,390,500,440);
  line(550,400,500,440);
  line(565,415,500,440);
  
  noStroke();
  eye(300,440);
  eye(500,440);
}

void eye(int x, int y){
  float a; 
  a = atan2(mouseX, mouseY);
  fill(255,255,255);
  ellipse(x, y,120,80);
  fill(0,0,0);
  ellipse(x + 13*cos(a), y + 13*sin(a),55,55);
}
