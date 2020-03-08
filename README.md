# UAAS Mods

UnityModManager 0.21.4 supported; Add the following to the UnityModManagerConfig.xml:

```
	<GameInfo Name="Ultimate Admiral Age of Sea">
		<Folder>Ultimate Admiral Age of Sea</Folder>
		<ModsDirectory>Mods</ModsDirectory>
		<ModInfo>Info.json</ModInfo>
		<GameExe>build.exe</GameExe>
		<EntryPoint>[UnityEngine.UI.dll]UnityEngine.EventSystems.EventSystem.cctor:After</EntryPoint>
		<StartingPoint>[Assembly-CSharp.dll]UltimateAdmiral.UI.MainMenuController.Init:Before</StartingPoint>
	</GameInfo>
```

Download and Install the CheatMod.zip file from the git repo. Use the Unity Mod Manager UI to change settings


CheatMod:
- Speed Button Multiplier (Changes speed multiplier value by this multiplier, making game go faster) (* A bit janky with the way the UI controls works. Just visual bug though.)
- Minimum Reputation
- Minimum Gold
- Inf Rifle/Cannon shop stock (Buy once to update)
- Inf Rifle/Cannon armory stock (Buy once to update)
- Take No Damage (Land)
- Max Condition (Land and Sea)
- Max Morale (Land and Sea)
- Max Supply (Land)

Equipment Mod:
- Edit stats of all rifles
- Edit stats of all ship cannons
Instructions:
Install the Equipment mod using UnityModManager, start the game and load up a save. Loading a game will cause the mod to export the Rifles.txt and Cannons.txt files to the Mod's install folder inside the game directory. Exit the game, and open the two text files. You can edit the stats
of the items here. When the game is loaded again, the mod will read these files and apply them to the items.
Do not edit the 'ID' property, as it is needed to apply properly. Editing the equipment description or name is not yet supported. 