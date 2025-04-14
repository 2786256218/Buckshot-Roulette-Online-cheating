# Buckshot-Roulette-Online-cheating
This item is used to implement cheats in Buckshot Roulette multiplayer mode to see the current remaining bullet types. The project is similar to https://github.com/Lou1sL/BuckshotRouletteClairvoyance
。

Note: Please split the packaging exe and do not integrate it.

Note: This project is only applicable to the current host, and the user needs to create the host himself to take effect, and it will be invalid if you join someone else's server.
Press the Q key to use the cheat feature
Of course, we will use Godot unpacking tool Godot PCK Explorer to unpack, https://github.com/DmitriySalnikov/GodotPCKExplorer

```GDScript
var mouse_pos
func _input(event):
	if event is InputEventMouse:
			mouse_pos = event.position
	if Input.is_key_pressed(KEY_Q):
		if MAIN_active_sequence_dict.has("sequence_in_shotgun"):
			var shellStr = "弹药序列: "
			var index = 1
			for shell in MAIN_active_sequence_dict.sequence_in_shotgun:
				if index > 1:
					shellStr += " → "
				if(shell == "live"): 
					shellStr += "致命"
				else: 
					shellStr += "空弹"
				index += 1
			for property in instance_handler.instance_property_array:
				if property.socket_number == MAIN_active_current_turn_socket:
					property.dialogue.ShowText_ForDuration(shellStr, 3)
```
Put the code after line 89 in the ".\multiplayer\scripts\global scripts\MP_GameStateManager.gd" file

<img width="916" alt="image" src="https://github.com/user-attachments/assets/27ac4893-8ef5-4c32-b312-523995b8c63d" />

Then save it

## Lazy approach
Download and replace the MP_GameStateManager.gd file I made to the unpacked directory ".\multiplayer\scripts\global scripts"

Finally, repackage your source code


