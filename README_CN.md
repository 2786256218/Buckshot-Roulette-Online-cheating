# Buckshot-Roulette-Online-作弊
该项目用于在Buckshot Roulette多人模式中实施作弊，以查看当前剩余的子弹类型。该项目类似于 https://github.com/Lou1sL/BuckshotRouletteClairvoyance。

注意：请拆分打包 exe，不要集成。

注意：本项目仅适用于当前主机，需要用户自己创建主机才能生效，如果加入别人的服务器将无效。按 Q 键使用作弊功能

回到正轨，同样的我们将使用 Godot 解包工具 Godot PCK Explorer 来解包，https://github.com/DmitriySalnikov/GodotPCKExplorer

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

将代码放在 ".\multiplayer\scripts\global scripts\MP_GameStateManager.gd" 文件中第 89 行之后

<img width="916" alt="image" src="https://github.com/user-attachments/assets/27ac4893-8ef5-4c32-b312-523995b8c63d" />

最后保存即可

## 懒惰的方式
下载并替换我创建的 MP_GameStateManager.gd 文件到解压后的目录 ".\multiplayer\scripts\global scripts"

最后，重新打包源代码


### 如果以上方法不会使用请移步至Releases下载我打包好的二进制文件
