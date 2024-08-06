let cor;
let posicaoHorizontal; // x
let posicaoVertical; // y

function setup() {
  createCanvas(800, 800);
   background(color(20,30,110));
  cor = color(900)
  posicaoHorizontal = 200;
  posicaoVertical = 200;
}


function draw() {
  
  fill(cor);
  circle(posicaoHorizontal,posicaoVertical,50);
 
  
  
  if (mouseX < posicaoHorizontal){
    posicaoHorizontal =  posicaoHorizontal - 1;
  }
  
  if (mouseX > posicaoHorizontal){
    posicaoHorizontal =  posicaoHorizontal + 1;
  }
  
  if (mouseY < posicaoVertical){
    posicaoVertical--;
  }
    
  if (mouseY > posicaoVertical){
    posicaoVertical++;
  }
   if (mouseIsPressed){
    cor = color(1000)
  }
 
}
