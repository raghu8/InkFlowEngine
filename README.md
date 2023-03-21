﻿# InkFlowEngine

  Ink flow engine is designed to orchestrate a set of actions on objects within a game. User will write a script and engine will analyze the script and look for verbs and nouns to determine what action to take and what object the action should be taken on. Verbs, nouns and preposion will be marked in a unique way in the script.  In the scenario below the main player is called Bob and he will go to a defined destination and interact with an object. 
  
  ActionScript
  
  ${Bob} [walks] (towards) the <tree>
  
  
  Characters and npc's are identified via ${}
  verbs are identified via []
  prepositions are identified via ()
  non character nouns are identified via <>
  
  
  Note: This is initial brain storm and is subject to change.
  
  
  
  Ideally this will be designed to work with unreal engine. Specifically this will be designed to orchestracte cutscenes to reduce animation work. That being said we will need a collection of animations to perform actions. In the example above "${Bob} [walks] (towards) the <tree>", this sentence should trigger the walk animation on bob. Target will move towards the tree (this is handled by unreals navmesh and ai).
  
  

Once desireable set of actions have taken place in the scene, these will be recorded and shipped out as cutscenes for the game.
Note: Since unreals navmesh and AI are being used, consistent outputs may be guaranteed but consistent movements cannot so it is recomended each script is recorded.



TODO: Brain storm more features or improve upon above
