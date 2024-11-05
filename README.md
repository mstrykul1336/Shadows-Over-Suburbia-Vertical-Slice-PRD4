# Shadows Over Suburbia Vertical Slice PRD4
**11/4/24:**
**What was done:**
- serialized all of the timers and added to check if master client before any coroutines are called. 
- changed party name to town name in the menu to fit aesthetic 
- made it so you can use escape for settings menu 
- made a mouse sensitivity slider in the settings so players can change mouse sensitivity
- changed all canvas UI to 1920 x 1080 and tried to lock all UI to their respective places. 
- changed the build resolution to 1270 x 720 to match the UI and still make it visible in the WebGL build. (1920 x 1080 made it too big to play)
- added more lighting and changed a lot of the lighting to white. this lighting will be changed when I change all the models
- made new 2D pixel sprites for all of the abilities and used them in place of the demo assets
- added a new red, bloody cursor 
- created a photon hashtable to store player roles and abilities 
- made another win screen for the old man if he wins and coded it in. 
- added in a bunch of new environment props and objects to the town hall room 
- added in a bunch of new environment props into every player's night room
- changed code for winning and losing to include old man's neutral alignment screen and hopefully by using the hashtable, the mechanic should work better. 
- changed the role reveal function to use the hashtable instead of trying to find the role in player controller list
  
**To Do:**
  
- I added in the how to play a different method of the voting system that is used in other games similar to mine. I want to implement this: 
- First round of voting will be held, where a player is selected to be voted out.  
- Then, another voting round will be held to either vote out the player or not. The player should get 30 seconds to make their case before players vote.  
-serialize timers and make sure any coroutine is always checking for the master client to do it, so hopefully this fixes any timer glitches.  
- make all UI scale to screen size with a screen size of 1920×1080. This includes locking the UI in certain places (From User Stories 3: As a player with bad eyesight, I would like the UI to lock to the corners, so that it is easier to read and I can see the center of the screen.) 
- make the HUD nicer and cleaner, making it easier to understand what’s going on and what you need to do. (From User Stories 3: “As a player who likes being given information, I would like the HUD to be a bit more organized so its not in my way and readable”). 
- try to make player list look nice and make sure the mayor icon displays for all players, not just for the mayor. 
- make UI to change mouse sensitivity in the settings wheel (From User Stories 3: “As a player, I would like to be able to change mouse sensitivity. “ ‘As a player who is picky with gameplay settings, I want an options menu so that I can adjust my mouse sensitivity and screen brightness”) 
- if mouse sensitivity does not fix the issues, consider and mess with changing the game from first POV to third POV (even though this isn’t my intended player experience, it may help with confusion, mouse clicking, etc). (From User Stories 3: “As a player, I would like there to be a secondary option to either move the camera or click using the mouse, so that I have an easier time clicking on things without my camera being weird or mouse locking.”)  
- winning and losing seems to be weird, where it sometimes wins if the sides are correct and sometimes doesn’t. I need to make sure this code is clear on winning and losing. (I am assuming it’s not correctly taking the alignments of players and still keeping dead players in count, so I will check there first. ) 
- newspaper role is just saying mayor no matter what their actual role was. Change how this works to properly implement what role the player was.  
- change the lighting in the rooms to a brighter direct light and use the red as spotlights to make the room clearer to see. (User Stories 3: “As a player who is picky with gameplay settings, I want an options menu so that I can adjust my mouse sensitivity and screen brightness”) 

