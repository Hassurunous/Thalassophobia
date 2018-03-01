## Table of Contents
  * [Game Design](#game-design)
    * [Objective](#objective)
    * [Gameplay Mechanics](#gameplay-mechanics)
    * [Level Design](#level-design)
  * [Technical](#technical)
    * [Scenes](#scenes)
    * [Controls/Input](#controlsinput)
    * [Classes](#classessks)
  * [MVP Milestones](#mvp-milestones)
    * [Week 1](#week-1)
    * [Week 2](#week-2)
    * [Week 3](#week-3)
    * [Week 4](#week-4)
    * [Week 5](#week-5)
    * [Week 6](#week-6)

---

### Game Design

#### Objective
Journey through the dark depths of the ocean and defeat the creature that stalks you. An exploratory mission turned tragic, you are trapped beneath the waves, with a limited supply of air, and no communication with the outside world. No way out, and a creature prowling the depths around, how long can you last? A narrative experience of terror and dread. Think: underwater horror escape room.

#### Gameplay Mechanics
The player moves through the environment using a "swim jet", which propels them in the direction they point their hand by squeezing the trigger. The player attempts to hide behind obstacles and plants as a dark shape moves through the water around them. Audio queues will show the player that they are running low on oxygen, and vision will start to fade as oxygen gets low. Their only hope of survival is returning to the surface, but if they try to move before killing or scaring off the creature that hunts the depths, they will be eaten before they can escape.

#### Level Design
A singular level. The bottom of the ocean, with a small ship far above. The player drops slowly into the ocean towards the ocean floor far below. After a few moments of exposition and setup, the player lands upon the floor of the ocean, and is taught how to move and use the controls. The air pump cuts off abruptly, and the character begins to hyperventilate. The oxygen percentage meter shows levels falling rapidly before the sounds of the pump begin again a few moments later. "Sorry about that! Keep calm and try not to panic if that happens. With all the air in that suit you should be able to spend several minutes without the pump before the air starts to get thin, and it only takes a few seconds to restart the pump, so you'll be fine," the voice calls over the comms. "Head that way " (a nav marker points the way) "to get to the dig site. Don't forget to grab your tools. With luck, we've got ourselves a chance to unearth some valuable artifacts before someone else notices the site. Still can't believe we found it after that earth quake. It's not every day you get a chance to crack open an ancient pyramid beneath the triangle. Superstitious idiots probably won't find it for weeks, but I'd rather get everything we can out of here before they do."

Player picks up a tool chest of some kind and swims over to the marker. "Good. You're almost there. Keep going. Just a bit further down." Player keeps swimming and eventually sees the pyramid looming as a silhouette in the water. As they approach, a shape detaches itself from the top of the pyramid. "Did you see that? I've got something on the radar moving above you. Watch your head." A massive shape undulates through the water just around the player's oxygen tube. "Is that a whale or something? Hard to tell on this old piece ah shit. Doesn't matter, keep going. You're almost to the doorway we scouted out earlier with the drone. You should see the glow sticks we dropped to mark the entrance."

As the player heads into the tunnel marked by the glow sticks, it grows too dark to see, with the entrance growing smaller behind them. Soon, a noise is heard in the water, as if a massive creature is screaming beneath the waves. "What the hell was that?! Did you see that thing?! Oh god! What is that thing?!" Gunshots ring out over the comms. Screams and cries of help. Static fills the channel and the creature screams again. The player watches as the ship sinks beneath the water, silhouettes of bodies and clouds of blood around it. A tentacle grabs ones of the bodies and drags it away. Their line goes slack. The pump is silent. The static stops.

As the player fights their way to the surface, the creature can be seen snatching bodies and other flotsam around them. They have their swim jet and a single harpoon. Can they fight their way to the surface? Will they run out of air? Will they be eaten by the creature?
[Back to top ^](#)

---

### Technical

#### Scenes
* Main Screen
* ...

#### Controls/Input
Pick up items with the grip button, and utilize those items with the trigger. Swim Jet can be used to propel yourself through the water. Harpoon gun can be shot. Spears can be used to stab. Oxygen tanks can be used to extend air supply.

#### Classes/SKS
* Classes
  * [list classes needed and some basic information about required implementation]
  * ...
* Scenes
  * [list Scene files you will need to create]
  * NarrativeScene

[Back to top ^](#)

---

### MVP Milestones
[The overall milestones of first playable build, core gameplay, and polish are just suggestions, plan to finish earlier if possible. The last 20% of work tends to take about as much time as the first 80% so do not slack off on your milestones!]
* Player can move around in the environment in 3 dimensions using the swim jet.
* Player can pick up and drop objects using the grip buttons
* Player cannot drop the swim jet (automatically returns to belt)
* Player can shoot the harpoon gun
* Enemy swims around the environment
* Player can hide from the enemy by blocking line of sight
* Player can kill injure and scare off the enemy (temporarily) with the harpoon gun
* Player can swim to the surface

#### Week 1
_MVP pre-setup_
* [goals for the week, should be build the game mechanics and objectives]
* Building the initial functionality for TapTargets
* Creating the sprite sheet for the first Player sprite
* Creating the sprite sheet for the first Enemy sprite
* Creating animations for the player and the first enemy
* Set up the default animation for the player and enemy

#### Week 2
_finishing a playable build_
* [goals for the week, should be finishing a playable game]
* Implement the UI/UX design into Unity - [3 hours]
	* Create each of the screens we will need (Main Menu, Combat, Shop, Map) - [½ hour]
	* Lay out each scene according to paper prototype - [1 hour]
	* Extra time in case something takes longer - [1 hour]
* Code core game loop. Creating TapTargets, controls, and behavior of the hero character. - [2 days]
	* Create TapTarget scoring functionality - [1 hour]
	* Create character and initial behavior - [1 hour]
    * Create enemy and initial behavior - [1 hour]
	* Core game loop - [4 hours]
		* Get tapping damage the enemies	- [2 hours]
		* Get enemies to spawn and approach the player - [1 hour]
* Validate core gameplay is fun - [1 hour]
* Plan out the animations that we want to implement. Idle, Attack, Run, Hurt, and Die for each character used. - [2 hours]
* Plan out short-term and long-term animation goals. - [½ hour]

#### Week 3
* [goals for the week]
* Finalize UI/UX design and layout - [About 1 day (with testing)]
* Get Animations implemented and triggered correctly - [½ day to 1 day]
* Implement points and health bar - [2 hours]
* Implement death - [2 hours]
* Start on Increasing Difficulty Levels, Shop, and Map - 1 day+
* Contain the probabilities of dropping health potions and armor refresh objects. [1 hour]
* Comment the implementation of the Shop and Map class - [1 hour]

#### Week 4
_polish and extra features_
* [goals for the week, should be finishing all core gameplay]
* Finish the Difficulty scaling, Shop, and Map - [1-2 days]
* Get persisting user high scores working - [2-3 hours]
* Adding Facebook login - [2-3 days]
 * Setting up online database account - [½ day]
 * creating database for highscore and linking it to the app - [½ day]
 * linking game with facebook sdk and getting login working - [½ day]
 * getting facebook accounts/score to the database via the game- [½ day]
* Persistent “saved” high score load to database - [½ day]
* Display leaderboard with other friends high scores - [½ day]
* Add analytics - [½ day]

#### Week 5
_submitting to the App Store_
* [goals for the week, should be finishing the polish -- demo day on Saturday!]
* Finalize with user testing and make sure all features are working as intended. -1 day
	* Have at least 5 and most preferably 10 students use my game and give feedback - [½ day]
* Make sure all credits are attributed in a credit scene. -½ day
* Apple developer account and certificates are set up and ready for submission. -2 hours
* Android Google Play Store account set up and tested
* Get ready to upload to the App Store / Google Play Store : [2 days+]
* Create screenshots for all device sizes supported - [½ day]
* Write out documentation for app stores - [½ day]
* Work out a presentable icon for the desktop screen - [½ day]
* Work out information/payment for developer account - [½ day]

[Back to top ^](#)
