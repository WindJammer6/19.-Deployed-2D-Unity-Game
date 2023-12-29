# 19.-2D-Unity-Game :bird:🏰
While trying to develop a 2D Unity game for a friend of mine (Github: [WolfPark](https://github.com/wolfparktaerim)), I thought that while my friend decides on the art aesthetics of the game, I could further familiarise myself with the process of creating a Unity game by creating a prototype 2D Unity game in advance, with sprites I found from Googling as a placeholder for the art aesthetics. This 2D Unity game can serve as the foundation for any further possible developments in the video game [WolfPark](https://github.com/wolfparktaerim) is trying to develop.

Here is the link of the deployed 2D Unity game on '[itch.io](https://itch.io/)': https://windjammer6.itch.io/2d-unity-game-by-windjammer6 (Click the link to play the game!)

Here is a demonstration of 'winning' the 2D Unity game, when the player successfully find the legendary sword:


https://github.com/WindJammer6/19.-2D-Unity-Game/assets/98175995/214bc246-3191-4908-95a5-9f5b54e82734



Here is a demonstration of 'losing' the 2D Unity game, when the player's health reaches zero:


https://github.com/WindJammer6/19.-2D-Unity-Game/assets/98175995/0d0364c2-50fb-4e1c-815c-3e8986bcbbfc



These videos are done by me, using [OBS Studio software](https://obsproject.com/) for screen recording and [VideoPad Video Editor](https://www.nchsoftware.com/videopad/index.html) (by NCH Software) for video editing.

Disclaimer: This 2D Unity game does not work for mobile, only for laptop, PC, or basically any electronic devices that has a keyboard since the game only detects key presses from a keyboard in order to move the character. It does not detect touchscreen controls. (idk how to do that yet, but I believe shouldn't be too difficult) You can open the 2D Unity game on mobile, but you will have no way to move the character.

<br>

### Features of the 2D Unity game:  
For this prototype 2D Unity game, there is a very vague storyline, as I did not dwell too much on that, but it is more focused towards adding various interesting features via C# programming into the game. Here is a list of features in the 2D Unity game:  

*Character-related:*  
1. Horizontal movement (left and right)
2. Jumping movement
3. Combat system, via dealing damage to enemy NPCs by firing projectiles ('bow' and 'arrow')
4. Health system (3 lives) (can take damage from enemy NPCs)

*Friendly NPC-related:*  
1. Interact with NPCs
2. Chief NPC can give the 'bow' weapon to the character

*Enemy NPC-related:*  
1. Chase character when the character enters their trigger range
2. Combat system, via dealing damage to the character when they come into contact with the character
3. Health system (3 lives for small enemies, 5 lives for big enemies) (can take damage from projectiles fired by the character)

*Background-related:*
1. Constructed the different sections of the 2D Unity game map, 'Village', 'Open Plains', 'Forest', and the final area with the legendary sword
2. Cloud movement
3. AI generated music on loop, generated by [AIVA](https://www.aiva.ai/)

*Game Objectives-related (in time order of the game):*  
1. Find a way to leave the castle-village (the castle-village's main gate is initially blocked, which you will be prompted by the Guard NPC that you need to interact with the Chief NPC to get the 'bow' weapon, before the blockage at the castle-village's main gate is removed and you can leave the castle-village)
2. Survive the forest with enemies using the 'bow' weapon (if the character loses all its health then you will lose the game)
3. Obtain the legendary sword at the end of the level to clear the game successfully

<br>

## Table of Contents
Here is a directory of this 'REAME.md' file:
1. [Game Idea](#gameidea)
2. [Building Process of this 2D Unity Game](#buildingprocess)
3. [Deployment Process of this 2D Unity Game](#deploymentprocess)
4. [Potential Improvements to this 2D Unity Game](#potentialimprovements)
5. [Technicalities between Unity and Github](#unityandgithub) 
   - [How to upload a Unity game into Github?](#howtoupload)
   - [How to download and use this Unity source code on Github in your Unity editor/software?](#howtodownloadanduse)

<br>

## 1. Game Idea <a name = "gameidea"></a>  
The design of this 2D Unity game is heavily inspired from the [original (OG) Super Mario Bros.](https://supermarioplay.com/) and [Genshin Impact](https://genshin.hoyoverse.com/en), both games that I have played before, with also many aspects of the initial ideas of the game from my friend, [WolfPark](https://github.com/wolfparktaerim). 

*Aspects of the 2D Unity game inspired by the [OG Super Mario Bros.](https://supermarioplay.com/):*  
- The 2D level design
- Character movement
- Enemy NPC behaviour 
- Health system and damage system
- The pixel-style art aesthetics

*Aspects of the 2D Unity game inspired by [Genshin Impact](https://genshin.hoyoverse.com/en):*  
- Friendly NPC interaction feature
- Interaction-related game objective (e.g. the '1. Find a way to leave the castle-village' game objective)

*Aspects of the 2D Unity game inspired by [WolfPark](https://github.com/wolfparktaerim):*  
- The story of the 2D Unity game (though I did not make it as detailed)
- The idea for the respective areas of the 2D Unity game, of a 'home' area, a forest with enemies, and an end objective (Also, [WolfPark](https://github.com/wolfparktaerim) wanted a boss fight, but it took too much effort, so eventually I made the end objective a less programming-intensive one, finding and claiming a 'prize')
- Recommendation of a copyright free, [AIVA](https://www.aiva.ai/) AI music generator, which I used to generate a suitable music for this 2D Unity game

*Source(s):*  
nil

<br>

## 2. Building Process of this 2D Unity Game <a name = "buildingprocess"></a>
This 2D Unity game is built on the [Unity](https://unity.com/) game development framework, so obviusly the building process is mainly done in the [Unity](https://unity.com/) editor/software, with the C# script components scripting done on the [VS code](https://code.visualstudio.com/) IDE. 

<br>

**About the folders that make up this 2D Unity game:**  
In reality, my Unity project/game is made up of the following folders:  
- Assets
- Library (not present in repository)
- Logs (not present in repository)
- Packages
- ProjectSettings
- UserSettings (not present in repository)

However, you might noticed that there are some folders that should be there that makes up my Unity project/game that aren't present in this repository such as the 'Library', 'Logs' and 'UserSettings' folders. See the section *'How to upload a Unity game into Github?'* in *'Technicalities between Unity and Github'* below for the reason.

+ The 'Assets' folder is the most important folder that contains the various files and resources used to create and run a Unity project/game, including 3D models, textures, scripts, audio files, animations, and more. The 'Assets' folder is also the root directory for your Unity project, and it organizes all of these assets in a hierarchical structure. For this 2D Unity game (since the type of folders in this 'Assets' folder varies for each Unity project/game), the 'Assets' folder contains 4 seperate folders, 'C# Scripts', 'Music', 'Scenes' and 'Sprites'.
+ The 'Packages' and 'ProjectSettings' folders are auto generated folders by Unity as you create a Unity project/game. Not super sure what exactly it is they do, but they are required and are not to be modified to prevent any bugs. They are required to be imported together with the most important 'Assets' folder,  into the Unity editor/software from Github in order to recreate a Unity project/game. See the section *'How to download and use this Unity source code on Github in your Unity editor/software?'* in *'Technicalities between Unity and Github'* below for more details.

<br>

**About the 4 folders in the 'Assets' folder of this 2D Unity game:**  

<br>

*C# Scripts:*  
Contains the C# scripts used in this 2D Unity game.

Despite taking the time to learn Unity's C# syntax as documented in my '[16.-Csharp-and-Unity-Learning](https://github.com/WindJammer6/16.-Csharp-and-Unity-Learning)' repository, that is only but a fraction of the Unity C# syntax. 

So most of these C# scripts are actually generated by [ChatGPT](https://chat.openai.com/), while I modified them while fixing their bugs, based on what I know about the C# programming language and the Unity C# syntax, to fit the requirements of this 2D Unity game.

(Note: 
What are these '.meta' files in my 'Assets' folder that are being created along with my Unity(C#) assets and why are they created? 
In Unity(C#), '.meta' files in the 'Assets' folder store the import settings of the assets/files in that 'Assets' folder in your Unity(C#) project. They tell the Unity(C#) editor/software how to prepare the asset/file in the 'Assets' folder in your Unity(C#) project. 

If you delete a '.meta' file, Unity(C#) reimports the asset and creates the default '.meta' file for that file type. Hence, it is advised that you don't delete them as the recreated default '.meta' file may not be the exact same as the initial '.meta' file that you deleted, potentially leading to missing behaviour errors. (Here is the source link of this information, from a Stack Overflow discussion on 'What is a .meta file and why does Unity create them for all of my assets?': https://stackoverflow.com/questions/42462989/what-is-a-meta-file-and-why-does-unity-create-them-for-all-of-my-assets)

<br>

*Music:*  
Contains the music used in this 2D Untiy game.  
- An ambient-themed soundtrack created by [AIVA](https://www.aiva.ai/), an AI music generator, which is set on loop using a C# script in this 2D Unity game.

<br>

*Scenes:*  
Contains the Unity scenes used in this 2D Unity game.
- The only 2D game level/scene of this 2D Unity game

A Unity scene is a container that holds all of the GameObjects, assets, and other elements for a specific part or level of your game.

<br>

*Sprites:*  
Contains the sprites used in this 2D Unity game.  
- Bird sprite, which represents the character and NPCs is taken from the 'The Unity Tutorial For Complete Beginners' Youtube tutorial video by Game Maker's Toolkit (link: https://www.youtube.com/watch?v=XtQMytORBmM&t=1s).
- The rest of the image sprites are taken from Googling.
- Variations in colour of the sprites, and the 'red bird character sprite with the bow' sprite is done via [Photoshop](https://www.adobe.com/products/photoshop.html)
- Scaling of the sprites was done directly in the Unity editor/software itself.
- Text sprites are generated from an [online transparent text generator](https://www.picturetopeople.org/p2p/text_effects_generator.p2p/transparent_text_effect), created by Picture to People. 

<br>

**Steps of the Building Process of this 2D Unity game:**  
1. Creating the background level design and it's respective areas ('Village', 'Open Plains', 'Forest' and the final area with the legendary sword) (learnt how to do this from the 'How to make Super Mario Bros in Unity (Part 1) - Level Design' and 'How to make Super Mario Bros in Unity (Part 2) - Movement/Physics' Youtube videos by Zigurous (links: https://www.youtube.com/watch?v=GCkq6XqyJZg&t=1529s and https://www.youtube.com/watch?v=SPe1xh4D7Wg&t=3480s respectively))
2. Creating the player character GameObject, and attaching the required GameObject components (e.g. 'SpriteRenderer', 'BoxCollider2D', 'RigidBody2D', etc) and C# scripts to define its behaviours (excluding health and combat systems)
3. Attaching the C# script that tells the main camera GameObject to follow the position of the character during the game
3. Creating the friendly and enemy NPCs, and attaching the required GameObject components and C# scripts to define its behaviours (excluding the health and combat systems of the enemy NPCs)
4. Creating the friendly NPC interaction features, while incorporating the '1. Find a way to leave the castle-village' interaction-related game objective, and the '3. Obtain the legendary sword at the end of the level to clear the game successfully' interaction to 'win' the game
5. Creating the player character and enemy NPCs' health and combat systems
6. Creating the cloud movement and spawner feature (the code and idea for this feature is also taken from the 'The Unity Tutorial For Complete Beginners' Youtube tutorial video by Game Maker's Toolkit (link: https://www.youtube.com/watch?v=XtQMytORBmM&t=1s))  
*Editorial view of the cloud movement and spawner feature:*



https://github.com/WindJammer6/19.-2D-Unity-Game/assets/98175995/755ab70f-c03e-404d-b0d2-cb05385884ca


*Game view of the cloud movement and spawner feature:*


https://github.com/WindJammer6/19.-2D-Unity-Game/assets/98175995/ecd2ea31-160f-48bb-b2c9-22edc9b3ba4f




8. Creating a music player GameObject, which has the [AIVA](https://www.aiva.ai/) AI ambient music soundtrack and a C# script attached to it which tells the Unity editor/software to play the soundtrack on loop (learnt how to do this from the 'How to play background music in Unity' Youtube video by Tony Morelli (link: https://www.youtube.com/watch?v=eB3I4l0AED0&t=81s))
9. Adding the 'Congrats you found the Legendary Sword. Thanks for playing!' (winning) and 'Game Over' (losing) messages, player health tracker/label, and the 2D Unity game instructions' text sprites

(Note: As of now, I have been using a pretty sketchy method to get some of the features to work, which is by turning text sprites active or inactive in C# scripts via the '.SetActive()' Unity C# function based on a condition. E.g. Setting the 'Interact' text sprites active when the player character move into the trigger range of the friendly NPC, then setting them inactive when they leave the trigger range, and, using multiple text sprites layered over one another, then setting them active when needed and inactive otherwise for the dialogues.)

*Source(s):*  
+ https://stackoverflow.com/questions/42462989/what-is-a-meta-file-and-why-does-unity-create-them-for-all-of-my-assets (Stack Overflow discussion on 'What is a .meta file and why does Unity create them for all of my assets?')
+ https://www.youtube.com/watch?v=GCkq6XqyJZg&t=1529s (Zigurous) (Youtube video labelled 'How to make Super Mario Bros in Unity (Part 1) - Level Design' by Zigurous)
+ https://www.youtube.com/watch?v=SPe1xh4D7Wg&t=3480s (Zigurous) (Youtube video labelled 'How to make Super Mario Bros in Unity (Part 2) - Movement/Physics' by Zigurous)
+ https://www.youtube.com/watch?v=XtQMytORBmM&t=1223s (Game Maker's Toolkit) (Youtube video labelled 'The Unity Tutorial For Complete Beginners' by Game Maker's Toolkit) 
+ https://www.picturetopeople.org/p2p/text_effects_generator.p2p/transparent_text_effect (Picture to People) (A Transparent Text Generator, to generate the text sprites for this 2D Unity Game)
+ https://www.adobe.com/products/photoshop.html (Photoshop)
+ https://www.youtube.com/watch?v=eB3I4l0AED0&t=81s (Tony Morelli) (Youtube video labelled 'How to play background music in Unity' by Tony Morelli) 
+ https://www.aiva.ai/ (AIVA)
+ https://chat.openai.com/c/f45522bd-c449-4c7f-aebc-15d58cb1cd44 (ChatGPT)
 
<br>

## 3. Deployment Process of this 2D Unity Game <a name = "deploymentprocess"></a>
Honestly, the 'How To Build & Deploy Your Games With WebGL' Youtube video by GDTitans (link: https://www.youtube.com/watch?v=UK7SEoiSB2c) explains very clearly step by step on how to deploy a Unity project/game. There are various platforms where you can deploy your Unity project/game, however, I just followed and deployed on the same platform as demonstrated in this video, '[itch.io](https://itch.io/)'. Once deployed, I got a direct '[itch.io](https://itch.io/)' link to this 2D Unity game, which I can then share with others to try out this 2D Unity game.

- Here is the link of my '[itch.io](https://itch.io/)' account of the username:, 'WindJammer6' - https://windjammer6.itch.io/.
- Here is the link of this deployed 2D Unity game on '[itch.io](https://itch.io/)' - https://windjammer6.itch.io/2d-unity-game-by-windjammer6

*Source(s):*  
+ https://www.youtube.com/watch?v=UK7SEoiSB2c (GDTitans) (Youtube video labelled 'How To Build & Deploy Your Games With WebGL' by GDTitans)

<br>

## 4. Potential Improvements to this 2D Unity Game <a name = "potentialimprovements"></a>  
*Adding features:*  
+ Adding a boss fight
+ Adding a restart/respawn of the player character feature (maybe can set the respawn point at the 'Village' area in the 2D Unity game?) if chacacter dies, rather than just showing the 'Game Over' message
+ Adding a feature where the area name that the player character is currently at is only briefly showed rather than it being a fixed text sprite in the 2D Untiy game game level scene, with a transition of the music being played based on the area. (Possible to use some sort of invisible trigger GameObject, and a time delay with fading effect of the music soundtracks upon triggering the entering of a different area before playing the corresponding music of that area for a more smoother music soundtrack transistion.)
+ Adding a 'Main Menu' game scene (with a replay game and exit game options?) and a 'Safehouse' game scene (which allows the player character to regain health upon entering the 'Safehouse' game scene?) (might be able to do this by creating different 'Unity scene' files in the 'Scenes' folder within the 'Assets' folder in the Unity editor/software)
+ Adding animations to the sprites in the game (I managed to find a Youtube video by Alexander Zotov labelled 'Unity 2D Tutorial About How To Create Idle Walk And Kick Animations For Game From Sprite Sheet' that shows how I might be able to do this in the Unity editor/software (link: https://m.youtube.com/watch?v=msTvOG4w80I)) 

*Fixing bugs:*  
+ Fixing of the bug where the player character might sometimes rotate due to incorrect game physics
+ Fixing of the bug where friendly NPCs are affected and can be 'pushed' by the player character's projectiles even though they should desirably be unaffected by the projectiles (maybe can create an additional C# script, making use of the 'Physics.IgnoreCollision()' Unity C# function to ignore the collisions between the friendly NPCs and the projectiles, and attaching it to the friendly NPC GameObjects)
enemy NPC should not rotate or leave the ground or chase endlessly? and stop chasing and returning upon character going too far
+ Fixing of the bug where the player character can climb the high walls at the start and end of the 2D Unity game game level and leaving the game level map

<br>

## 5. Technicalities between Unity and Github <a name = "unityandgithub"></a>  
Once I completed this 2D Unity game, I wanted to be able to document the process of creating this 2D Unity game on Github, as well as being able to somehow upload the 2D Unity game files onto Github and re-download the 2D Unity game files to re-import them into my Unity editor/software. However, it took me quite a while to figure out how to upload a Unity game into Github and download and re-import Unity game source codes from Github into the Unity editor/software. So I thought I'll document how to do these 2 processes here as well.

<br>

### How to upload a Unity game into Github? <a name = "howtoupload"></a>
Honestly, the 'How to Upload your Unity Projects to GitHub In 2023' Youtube video by GDTitans (link: https://www.youtube.com/watch?v=YymhtHtHDb8&t=8s) explains very clearly step by step on how to upload a Unity project/game into Github. 

*A bit more about the '.gitignore' file in this repository:*  
In reality, my Unity project/game is made up of the following folders:  
- Assets
- Library (not present in this repository)
- Logs (not present in this repository)
- Packages
- ProjectSettings
- UserSettings (not present in this repository)

Which, you might have noticed that some of the folders are missing in this Github repository. This is because during uploading of a Unity project/game into Github as shown in the Youtube video, Github creates a special file called the '[.gitignore](https://github.com/WindJammer6/19.-2D-Unity-Game/blob/main/.gitignore)' file, which allows Github to ignore the files that are unnecessary for collaboration or version history such as files that are generated during the development process, temporary files, build artifacts, etc. for reasons such as for version control and saving space in Github's servers. In the context of Unity, such unnecessary files are the files in the 'Library', 'Logs' and 'UserSettings' folders, which are not required and are generated automatically anyway when you re-download and re-import the more important 'Assets', 'Packages' and 'ProjectSettings' folders into the Unity editor/software from Github (basically the remaining folders that I have provided here in this repository)

Taking a peek at the code in this '[.gitignore](https://github.com/WindJammer6/19.-2D-Unity-Game/blob/main/.gitignore)' file in Github for Unity:
```
# This .gitignore file should be placed at the root of your Unity project directory
#
# Get latest from https://github.com/github/gitignore/blob/main/Unity.gitignore
#
/[Ll]ibrary/
/[Tt]emp/
/[Oo]bj/
/[Bb]uild/
/[Bb]uilds/
/[Ll]ogs/
/[Uu]ser[Ss]ettings/
```

Which shows us the types of folder in a Unity project/game that the '[.gitignore](https://github.com/WindJammer6/19.-2D-Unity-Game/blob/main/.gitignore)' file in Github for Unity will ignore, which includes the 'Library', 'Logs' and 'UserSettings' folders.

*Source(s):*  
+ https://www.youtube.com/watch?v=YymhtHtHDb8&t=8s (GDTitans) (Youtube video labelled 'How to Upload your Unity Projects to GitHub In 2023' by GDTitans)

<br>

### How to download and use this Unity source code on Github in your Unity editor/software? <a name = "howtodownloadanduse"></a>
Honestly, the 'How to import GitHub projects into Unity!' Youtube video by Unity Hero (link: https://www.youtube.com/watch?v=I9QK_2QW9W8) explains very clearly step by step on how to download and use a Unity source code on Github in your Unity editor/software.

Initially, I managed to re-download and re-import this 2D Unity game from this 2D Unity game Giithub repository. However, when I re-opened the re-imported 2D Unity game in the Unity editor/software, I was super confused when the game scene in the Unity editor/software is empty and i thought I might have been missing an important folder that I should have uploaded into this 2D Unity game repository from my original 2D Unity game folder from the Unity editor/software in my computer. 

However, it turns out, which this Youtube video showed me, is just that I needed to go to the 'Scenes' folder within the 'Assets' folder in the Unity editor/software, and click on the default 'Unity scene' file titled 'SampleScene' to re-open the original game scene visually in the game view in the Unity editor/software, with all my GameObjects and C# scripts placed at where they should be as the original 2D Unity game's copy, without having to re-add them all manually, which I almost wanted to do 😢. 

*Source(s):*  
+ https://www.youtube.com/watch?v=I9QK_2QW9W8 (Unity Hero) (Youtube video labelled 'How to import GitHub projects into Unity!' by Unity Hero) 


