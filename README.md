var spaceshuttle;
function preload() {
  spaceshuttle = loadImage("https://img.pixers.pics/pho_wat(s3:700/FO/64/58/66/07/700_FO64586607_df3f84775b3bd25e95657ef9cbc1c996.jpg,490,700,cms:2018/10/5bd1b6b8d04b8_220x50-watermark.png,over,270,650,jpg)/stickers-raket-op-een-witte-achtergrond.jpg.jpg");
}
function setup() {
  createCanvas(400, 400);
  
}
// zwart gat
function draw() {
  background(0);
  noFill();
  stroke(250, 140, 0);
  strokeWeight(11);
  ellipse(200, 200, 100+sin(frameCount/10), 100);
  strokeWeight(11);
  arc(200, 210, 100, 100+sin(frameCount/2), 0, PI);
  stroke(255)
  fill(255)
  // Joek, ik heb het zo gedaan omdat mijn sterren anders in het zwarte gat gaan en dat wil je niet hebben.
  ellipse(200, 100, 9+sin(frameCount/20), 9);
  ellipse(150, 40, 9+sin(frameCount/20), 9);
  ellipse(50, 200, 9+sin(frameCount/20), 9);
  ellipse(80, 100, 9+sin(frameCount/20), 9);
  ellipse(300, 350, 9+sin(frameCount/20), 9);
  ellipse(340, 230, 9+sin(frameCount/20), 9);
  ellipse(340, 100, 9+sin(frameCount/20), 9);
  ellipse(50, 340, 9+sin(frameCount/20), 9);
  ellipse(90, 300, 9+sin(frameCount/20), 9);
  noStroke();
  fill(64, 40, 34);
  ellipse(200 + sin(frameCount/100) * 150,
      200 + cos(frameCount/50) * 300, 40, 40);
  ellipse(200 + sin(frameCount/50) * 150,
      200 + cos(frameCount/50) * 100, 30, 30);
 image(spaceshuttle, mouseX, mouseY);
  
}
