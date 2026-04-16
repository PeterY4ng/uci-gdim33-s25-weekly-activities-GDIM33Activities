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


## W2
<img width="1440" height="1002" alt="image" src="https://github.com/user-attachments/assets/9e0cbc5c-45e1-48c5-a747-5716941f052b" />

This avoids hard-coded strings. If I need to change the event name later, I only have to modify the value of this single variable instead of searching everywhere to update every place that triggers the event. This makes the project easier to maintain and less prone to errors.
When clicking the walrus, Debug.Log("Walrus Clicked!") prints a message to the Console, confirming that the click event was successfully triggered. The log messages in the transitions also verify that the state changes worked correctly, allowing me to quickly identify where the logic failed — for example, whether the click didn’t register, the event wasn’t sent, or the transition didn’t execute.
Is the Set Cursor Lock State relevant to your Vertical Slice?
Not really. In my game, the Explore state uses a third-person / movement perspective, so locking the cursor to prevent it from moving outside the window is not necessary.
The concept of game states is highly relevant. My game has two distinct modes: combat/movement and interaction. Using a state machine keeps the logic for these modes separate and prevents conflicts — such as not being able to attack during interactions or trigger dialogue buttons while attacking. It also makes the overall logic clearer and easier to maintain.


Continue adding additional headers below this one for future weeks and future activities.
