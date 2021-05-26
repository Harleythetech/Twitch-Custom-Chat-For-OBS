# Twitch-Custom-Chat-For-OBS
This repo is deisgned to work with twitch chat for OBS (using Browser source)

I Discovered this while Experimenting with Dev Tools In Microsoft Edge 

--------------------------------------------------------------------------
Instructions on how to change everything 

First Open OBS once it's open Locate your Browser source/TChat the right click and click on properties
Once your in locate Custom CSS then Open the code you downloaded using notpad or Notepad++ (recommended)
Copy the code and paste it in the Custom CSS section In OBS
Like this:
![Screenshot 2021-05-26 202314](https://user-images.githubusercontent.com/51787264/119659939-42fe4f80-be61-11eb-8405-030490ee932c.png)

after this you can change every value to what you desired (full on instruction bellow)

--------------------------------------------------------------------------
First part Of code:
--------------------------------------------------------------------------
    html, body,
    .room-selector, .room-selector__header,
    .twilight-minimal-root, .tw-root--theme-light,
    .popout-chat-page, .chat-room, .tw-c-background-alt,
    .chat-container, .ember-chat-container {
    
      background: rgba(0,0,0,0)!important; 
THIS PART IS IMPORTANT AND IS RESPONSIBLE FOR MAKING CHAT TRANSPARENT
    
      background-color: rgba(0,0,0,0)!important;  
    }
SAME AS BG THIS IS RESPONSIBLE FOR MAKING CHAT TRANSPARENT
    

--------------------------------------------------------------------------
ON TO NEXT CODE WHERE THE MAGIC HAPPENS :D

--------------------------------------------------------------------------
SIMPLEBAR CONTENT IS RESPONSIBLE FOR THE CHAT FONT, COLOR, SIZE IF YOU WANT TO CHANGE THESE FOLLOW THE INSTRUCTION TO AVOID ERRORS :D

--------------------------------------------------------------------------
(second part of code)
 
    .simplebar-content {
    
        font-size: 25px!important;  

TO CHANGE CHAT SIZE SIMPLY REPLACE THE "25px" number to what ever size you want Example: 13px
how to change: "font-size: 25px!important;" (always ignore "") and your all set! 
    
        font-family: UD Digi Kyokasho NK-B !important; 
    }

TO CHANGE CHAT FONT SIMPLY REPLACE "UD DIGI KYOKASHO NK-B" WITH YOUR DESIRED FONT
EXAMPLE: ARIAL " font-family: Arial !important; " (always ignore "") and your all set! 


--------------------------------------------------------------------------
(third and last code responbsible for the color of the font) ( lASTLY WANT TO CHANGE THE CHAT COLOR? WELL HERE'S HOW TO DO IT! )

    .tw-root--theme-dark .chat-line__moderation, .tw-root--theme-dark .chat-line__status, .tw-root--theme-dark .chat-line__message {

      color: #ffb6c1; 

    }
--------------------------------------------------------------------------
IN ORDER TO CHANGE COLOR YOU NEED TO CHANGE THE HEXCIDECIMAL CODE (HEX FOR SHORT) WHICH IS THE "#FFB6C1" TO CHANGE THIS
 YOU WILL NEED A HEX COLOR CODE (LINK TO WHERE TO FIND ONE WILL BE INCLUDED) SO LET'S SAY YOU FOUND THE COLOR YOU WANT EXAMPLE:  "#D4E6F1"
WHAT YOU WANT TO DO IS REPLACE "#FFB6C1" WITH "D4E6F1" (CLEAR INSTRUCTION BELOW)

-------------------------------------------------------------------------- 
HOW TO REPLACE:
 
    FROM: color: #ffb6c1;
    TO: color: #D4E6F1; 

--------------------------------------------------------------------------
AFTER THAT YOUR ALL SET! SAVE AND REFRESH AND YOU SHOULD 
SEE OBS WITH DIFFERENT COLOR, FONT, + TRANSPARENT BACKGROUND
Link to where you can find HEX color codes: https://htmlcolorcodes.com/

--------------------------------------------------------------------------
Made with Love <3
-Harleythegreaat, MysticMusic, Harley, Harleythetech 

--------------------------------------------------------------------------
