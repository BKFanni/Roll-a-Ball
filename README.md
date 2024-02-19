# Roll-a-Ball

Try out the game here: https://bkfanni.github.io/Roll-a-Ball/    :)

Implementation (Fanni & Marwa)

We implemented our first game individually, following a Unity learning path and added some extra functionalities on top of that
In the beginning it was a bit challenging to figure out and get used to the different tools and sections in Unity, and how to control the game objects
Beginning with setting up the game by creating a workspace for  the project and creating a new scene.
Then we added Rigidbody to the Player game object so it uses the Unity Physics Engine that enables the Player object to move according to the laws of physics.

Regarding writing the scripts, we have to create the logic for the behavior of game objects
By installing the input system package we can add input components to a game object that enables us to add input action assets.
We also added some basic configurations on the game objects, like where it is positioned in the scene and the color of the object, etc.
During development, when we added the Main Camera object as a child game object of the Player and tested the game, we noticed how the camera rotates with the movement of the Player GameObject. So to fix that we created a CameraController script that sets the position of the Camera object and follows the Player object with a fixed offset
Then we set up the Play area by creating walls so that the Player can move around but can only move in that area
 Creating Collectible GameObject was useful to learn how to make a game object rotate using the update function in the script ,and to make it as prefab to help us deal with multiple instances  from the same object.
 
In order to be able to simulate collecting the pickUp objects, we needed to add a script that deactivates (making it disappear) that specific object when the Player object hits it. For this we used the tag ‘pickUp’ for the pickUp object to make sure they are the only things that disappear. Then we set the prefab pickUp Collider as a trigger.
 In order for the player to know the progress that happened during the playing experience It suppose for the game to show the count of the pickup that the player successfully picked them up , so the game need to save score and show it as a UI text somewhere in the scene by Initialize the count variable in start function and Increment the count in OnTrigger Function 
One of the extra features we added to the game to make it more usable was the Restart Game button at the end of the game, after successfully collecting the 12 pickUp objects. It just reloads the scene to the active scene, so we get back to where we started. And the other one is the Quit Game button that just quits the application.
Building The Game is a very important step For exporting the game for the user or to try it with other people and to implement that we need to choose the Target Platform and add the Scene and from Player Settings it will open a range of different configuration options for the Game view, then we choose the Windowed instead of fullScreen because it make more sense for this type of game.

Reflection

(Fanni)
I think the tutorial was really useful for implementing my first game. It helped me to understand how to use Unity and how to add and implement different functionalities of a game. It gave me the fundamentals of how to start on making a game and it enables me to further develop my skills.

(Marwa)

Getting started with Unity to make my first game was super exciting! I've always been curious about game development, and Unity seemed like the perfect place to start.

At first, though, Unity felt like a big maze. There were so many buttons and sections to figure out, like the scene section and inspector. It was a bit overwhelming, but I kept at it and followed the tutorial. With time, everything started to make more sense.

The trickiest part for me was understanding how different parts of the game connect. I had to figure out which thing in the game should be connected to what, and how they should interact with each other. It took some trial and error, but eventually, I got it to work.

Another tough thing was controlling where objects go in the game. For example, making sure that objects like pick-ups appeared in the right place. It required me to be specific for 
 control positions, but I learned a lot along the way.

I know there's still a lot to learn, but I'm excited to keep practicing and getting better at making games with Unity.
