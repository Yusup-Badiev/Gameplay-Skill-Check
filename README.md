## Complete Game Play Task

This document outlines all the elements of the complete skill check code and how they interact:

## Button to open door
- There is a hidden button next to the building for unlocking the door. It is hidden by a script under its "Scripts" property.
- The script is set to "DOS2_PUZZLE_HiddenPerception" and adds a Perception check to the button.
- The button’s "Use Actions" property is set to "Send a use event to Osiris," allowing me to capture it in the Story Editor script. That script detects when the button is pressed, checks if the door is locked, and, if it is, opens the door.

## Key on goblin guarding the door
- There is a key that can be looted from the goblin at the door and used to unlock the door.
- The key unlocks the door because the "Key ID" on the key and the "Key ID" on the door are the same, meaning it can open the door.

## Dialog with goblin
- The goblin at the door has two possible dialog options. One sets the tavern fight flag and sets the goblin’s faction to evil when that flag is captured by the story script.
- The other option triggers an Intimidation roll. If the roll passes, the open tavern door flag is set and the door is unlocked for you. If the roll fails, the fight flag is set and a fight starts.

## Goblin Door Guard stats
- In the Stat Editor under my project name, I made a Door_Guard character stat and set the "Stats" attribute for the door guard to "Door_Guard."