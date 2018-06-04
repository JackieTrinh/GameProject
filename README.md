# GameProject
### Rocket Jump
### By Jackie Trinh

## Description

* This is a game I drew and programed in a month. 

## Instructions

* W to move up
* A to move left
* S to move down
* D to move right 
* SPACE BAR to shoot 
* MOUSE to aim 

### How to play the game 

* open the gamemaker executable to play the game. 

## Programs Used

Gamemaker Language 
* It's a simple language I like useing.

ColorZilla
* To get colors for the art.

Discord 
* I used this to download music from Noah who made music for the game and to talk with my friend Marcus who helped with the code. 

## Purpose

* In the future I want to be paid to make games so I made this program to show off what I can do.

## Function

* The function of this game is to be an enjoyable experence for the player to play.  

## Abstractions

* 

## Screenshots

![alt text](https://github.com/JackieTrinh/GameProject/blob/master/unknown1_opt.png)

![alt text](https://github.com/JackieTrinh/GameProject/blob/master/unknown2_opt.png)

![alt text](https://github.com/JackieTrinh/GameProject/blob/master/unknown3_opt.png)

## Gameplay Video
https://youtu.be/VnH7L-4vB8I

* Made with OBS, Blender and WMM

## Code Development

>//snow 

>if (script_execute(touching)) {

>//givning each snow a part in an array 

>for (i = 0; i < instance_number(obj_Psnow); i += 1) {
>    Psnow[i] = instance_find(obj_Psnow,i);
>    mult1[i] = clamp(1-(point_distance(x,y,Psnow[i].x,Psnow[i].y)/100),0,1);
    
>    if(mult1[i]<0.1) {
>        mult1[i] = 0;
>    }
>    //giving snow knockback
>   Psnow[i].hsp += ((clamp(Psnow[i].x-x,-15,15))*mult1[i])*(random(1)+0.5);
>   Psnow[i].vsp += ((clamp(Psnow[i].y-y,-5,25)-15)*mult1[i])*(random(1)+0.5);
>}

>}
