# Rain
My coding Journey
When I started to build this little prince project, my ultimate goal is to win a contest. Whatsoever, I started to do it. The first parts of my project is easy, since I don't need to write complicated lines. But when I started to do a toolbox, I met a problem:
             //variables
             var toolBox = false;
var Color = [255,255,255];

//button
draw = function() {
    ellipse(570,30,30,30);
    
if (toolBox === false && mouseIsPressed && mouseX >= 555 && mouseX <= 585 && mouseY >= 15 && mouseY <= 45&& mouseIsPressed){
    rect(500,10,90,560,20);
    toolBox = true;
    fill(255, 0, 0);
    ellipse(550,50,20,20);
    
    fill(255, 132, 0);
    ellipse(550,90,20,20);
    fill(255, 235, 0);
    ellipse(550,130,20,20);
    fill(114, 195, 0);
    ellipse(550,170,20,20);
    fill(50, 153, 213);
    ellipse(550,210,20,20);
    fill(157, 0, 255);
    ellipse(550,250,20,20);
    fill(255,192,203);
    ellipse(550,290,20,20);
    keyPressed = function() {
    //red
    if (key.code=== 114 && toolBox === true) {
        Color = [255,0,0];
    }
    if(key.code === 111&& toolBox === true) {
        Color = [255, 165, 0];
    }
    //yellow
    if (key.code === 121&& toolBox === true) {
        Color = [246, 190, 0];
    
    }
    //green
    if (key.code === 121&& toolBox === true) {
        Color = [103, 195, 0];
    
    }
    //blue
    if (key.code === 98&& toolBox === true) {
        Color = [50, 153, 213];
    
    }
    //purple
    if (key.code === 112&& toolBox === true) {
        Color = [157, 0, 255];
    }
    //pink
    if (key.code === 80&& toolBox === true) {
        Color = [255,192,203];
    }
};
}
    fill(Color);
    mouseDragged=function(){
    
    noStroke();
    ellipse(mouseX,mouseY,10,10);
    };
    
};


as you can see, I tried to change the colors of my paint brush by setting a variable and changing the variuable throughout. When I define a draw function like this, it will repeat infinitely. But I just can't figure out why it isn't work. You see, when I put a println into the if statement that controls the pink, it will appear. But when I try to drag the mouse, I find out that the color is always white. There must be some problem the change of my varible Color, but I don't seem to notice.
