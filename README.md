# Assignment 3: Making Beat Saber in Unity

**Due: Tuesday, October 12, 10:00pm CDT**

[Beat Saber](https://beatsaber.com/) is widely considered to be one of the best and most successful virtual reality games. There is a free demo available for the Oculus Quest, which you can find in the official store app. Before beginning this assignment, I suggest that you download this demo or watch some videos on YouTube to familiarize yourself with the gameplay.

In this assignment, you will be implementing Beat Saber's core mechanics. You can use Unity's built-in 3D objects (e.g. cubes) for this assignment, and you do not need to import custom meshes. If you want to make your game more interesting, you are also free to import additional assets. You can also modify any of the colors, textures, or lighting in the scene. Creativity is encouraged! However, note that your grade will be based on the interaction functionality, not the artistic quality of the game.

## Submission Information

You should fill out this information before submitting your assignment.  Make sure to document the name and source of any third party assets such as 3D models, textures, or any other content used that was not solely written by you.  Include sufficient detail for the instructor or TA to easily find them, such as a download link.

Name: 

UMN Email:

Third Party Assets:

Bonus Challenge Description (if applicable):

## Getting Started

Clone the assignment using GitHub Classroom.  The project has been configured for the Oculus Quest, and the [XR Interaction Toolkit](https://docs.unity3d.com/Packages/com.unity.xr.interaction.toolkit@1.0/manual/index.html) package has already been imported.  The scene contains the same room with two functional laser swords that are activated using the controller grip buttons, as described in [lecture 9](https://github.com/CSCI-5619-Fall-2021/Lecture-9).

## Rubric

Graded out of 10 points. 

1. Make a single cube that starts at the far end of the room and moves towards the user's start position.  Adjust the size and velocity so that it provides an appropriate challenge.  (1)
2. When the user hits a cube with a laser sword, the cube should be destroyed.  (1)
3. When the cube is destroyed, the user should be awarded points that 
4. Create a `CubeSpawner` that creates new cubes at random time intervals between 0.5 and 2.0 seconds.  You can feel free adjust these time thresholds to reach an appropriate difficulty.  The cubes should also start at the far end of the room, fly towards the user, and should be destroyed when hit by a laser sword. (2)
5. The exact X and Y positions of the spawned cubes should be chosen randomly, but should always be within reach of the user's swords when standing at the start position. (1)
6. If the cube collides with a wall, it should also be destroyed, but no points should be awarded.  We don't want to end up with infinite cubes that would slow down the application! (1)
7. Cube direction.
8. Left and right swords.

**Bonus Challenge:** TBD

Make sure to document all third party assets in your readme file. ***Be aware that points will be deducted for using third party assets that are not properly documented.***

## Submission

You will need to check out and submit the project through GitHub classroom.  **Make sure your APK file is in the root folder.** Do not remove the `.gitignore` or `README.md` files.

Please test that your submission meets these requirements.  For example, after you check in your final version of the assignment to GitHub, check it out again to a new directory and make sure everything opens and runs correctly.  You can also test your APK file by installing it manually using [SideQuest](https://sidequestvr.com/).

## Acknowledgements

This project uses a modified version of the [UnityLaserSword](https://github.com/jjxtra/UnityLaserSword) asset by Jeff Johnson (jjxtra).

## License

Material for [CSCI 5619 Fall 2021](https://canvas.umn.edu/courses/268490) by [Evan Suma Rosenberg](https://illusioneering.umn.edu/) is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-nc-sa/4.0/).

The intent of choosing CC BY-NC-SA 4.0 is to allow individuals and instructors at non-profit entities to use this content.  This includes not-for-profit schools (K-12 and post-secondary). For-profit entities (or people creating courses for those sites) may not use this content without permission (this includes, but is not limited to, for-profit schools and universities and commercial education sites such as Coursera, Udacity, LinkedIn Learning, and other similar sites).   