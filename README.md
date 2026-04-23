# GDIM 33 In-Class Activities
## W1
### Activity 1
https://docs.google.com/drawings/d/1wFLnbhUyBhbvpkCW6EMztMqo3PMJmFc-rnTfPY5FK54/edit

My inspiration sources mainly include the core features of three games: Soul Knight, Dead Cells and Neon Abyss.
First of all, I plan to make the game in pixel style. It is an art style that I personally love very much, and it is also the visual effect I want the final work to present. Secondly, this is a 2D game. Players can control characters in fixed map scenes, use various weapons and exclusive special skills to defeat monsters, and obtain in-game currency after clearing levels.
During the production stage, I will design multiple differentiated maps, original monsters and scene obstacles. Meanwhile, I will equip players with a rich variety of weapons and skill systems to enhance the playability of the game.

Most of my deskmates want to make roguelike games. Although I haven't decided exactly what game to make yet, most of the 2D pixel game resources I found are also of this type.

Our group TA is named Aaron. He likes playing multiplayer first-person shooter games such as Overwatch. Our gaming preferences are actually quite similar. The game I usually play, Valorant, is also a competitive multiplayer first-person shooter.


### Activity 2
![c22efe45c4a44ebef737ab5746843deb](https://github.com/user-attachments/assets/ecde11ab-02dc-4f21-87cc-f5cf31f20166)


## W3
<img width="1440" height="1002" alt="image" src="https://github.com/user-attachments/assets/9e0cbc5c-45e1-48c5-a747-5716941f052b" />

This avoids hard-coded strings. If I need to change the event name later, I only have to modify the value of this single variable instead of searching everywhere to update every place that triggers the event. This makes the project easier to maintain and less prone to errors.
When clicking the walrus, Debug.Log("Walrus Clicked!") prints a message to the Console, confirming that the click event was successfully triggered. The log messages in the transitions also verify that the state changes worked correctly, allowing me to quickly identify where the logic failed — for example, whether the click didn’t register, the event wasn’t sent, or the transition didn’t execute.
Is the Set Cursor Lock State relevant to your Vertical Slice?
Not really. In my game, the Explore state uses a third-person / movement perspective, so locking the cursor to prevent it from moving outside the window is not necessary.
The concept of game states is highly relevant. My game has two distinct modes: combat/movement and interaction. Using a state machine keeps the logic for these modes separate and prevents conflicts — such as not being able to attack during interactions or trigger dialogue buttons while attacking. It also makes the overall logic clearer and easier to maintain.


Continue adding additional headers below this one for future weeks and future activities.

## W4
### Activity 1
Playtest groupmates: Ruichen Ma, Alvin Wang, Gong Chen, Ziyue Yang(me)

In this playtest session, I have completed the basic dungeon map layout for my game. I also placed many jar obstacles inside the scene. Some jars can be destroyed normally by the player, while other jars cannot be broken at the moment. This issue is caused by small code errors, and I will fix these bugs in the next development stage.
I told the playtester the basic controls in advance. The player uses W, S, A, D to move the character, and the Spacebar is the interaction key to interact with objects and break jars. During the playtest, the tester quickly understood all the controls. The player could move smoothly using WASD and successfully use the Spacebar to break all destroyable jars. The basic movement and interaction work well with no major problems.
However, my current Vertical Slice does not have enemies, objectives, or a clear game ending condition yet. After the tester broke all the destructible jars in the scene, there was nothing left to do in the game. The gameplay experience was short, and there was no clear gameplay loop or goal. In the next step, I will add basic enemies, simple level objectives, and a basic ending system to improve the complete playable experience.

### Activity 2
1. Yes, the writer can fully add new dialogue content without writing a single line of code.
This is because the programmer has fully established the underlying operating logic and framework of the dialogue system through C# code and Unity Visual Scripting. When the writer needs to add new dialogue, they only need to create new dialogue node assets, fill in the dialogue text to be displayed, set up the player's optional response options, and link each node to its corresponding follow-up dialogue node — this is all it takes to complete a full new dialogue branch.
Throughout the entire process, the writer only modifies the content data of the dialogue, and never touches or alters the underlying operating logic of the dialogue system. For this reason, no code writing is required at all.

2. There is no hard technical upper limit on the number of dialogue nodes that can be created without writing code; Unity's ScriptableObject assets and Visual Scripting system are capable of supporting the creation of a vast number of dialogue nodes.
However, in practical development and application, there is a significant soft efficiency constraint. When creating a large volume of dialogue with complex branching — especially in scenarios where the same dialogue node needs to be reused with different branching options — the approach of relying solely on manually dragging nodes and linking dialogue chains will lead to extremely low efficiency.

3. Its main purpose is to refresh and complete the node library of Visual Scripting.When we write new custom C# classes ourselves or import code from third-party plugins, Unity’s default Visual Scripting does not automatically recognize these non-native classes, nor does it generate corresponding usable nodes for them. By clicking the "Regenerate Nodes" button at this point, it will automatically scan all newly added custom classes and third-party classes in the entire project, and then generate corresponding visual nodes for these classes.