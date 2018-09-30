# Processing_drawings-1


/* 
Your name: Elias Han

Date: 9/28/18

Project/assignment name: Java Sketch

Description: A sketch

Credits for code referenced: 
https://processing.org/tutorials/color/ 
https://processing.org/tutorials/pshape/ 

uses:
pshape
color
rectangle

*/

PShape rectangle;

void setup() {
  size(800,400,P2D);
  rectangle = createShape(RECT,-100,-50,100,50);
  rectangle.setStroke(color(50,50,255));
  rectangle.setStrokeWeight(4);
  rectangle.setFill(color(0,0,255));
}

void draw() {
  background(250,50,9);
  translate(mouseX, mouseY);
  rectangle.setFill(color(map(mouseX, 0, width, 0, 50)));
  shape(rectangle);

}
