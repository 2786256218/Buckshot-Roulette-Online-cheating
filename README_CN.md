# 操作步骤

下载 Godot PCK Explorer
https://github.com/DmitriySalnikov/GodotPCKExplorer/releases/download/1.5.3/GodotPCKExplorer_1.5.3_dotnet-ui-console-win-linux-mac.zip

首先启动Godot PCK Explorer

<img width="1276" alt="image" src="https://github.com/user-attachments/assets/9b1cd5db-4617-4049-92ae-0a9cc90ebefd" />

将Buckshot Roulette.exe导入进工具

<img width="1277" alt="image" src="https://github.com/user-attachments/assets/44c95740-9bad-4c4c-9bc8-40c8155b9fdd" />

选择该项

<img width="1277" alt="image" src="https://github.com/user-attachments/assets/75d84f12-9257-434b-8876-9585a6b46b75" />

选择一个空目录来保存文件

将下载后的MP_GameStateManager.gd文件替换到".\multiplayer\scripts\global scripts\MP_GameStateManager.gd"

在那之后选择该项来打包修改后的源代码文件

<img width="1277" alt="image" src="https://github.com/user-attachments/assets/52dab4b9-47a1-4d57-9f42-6e121724b019" />

<img width="1277" alt="image" src="https://github.com/user-attachments/assets/b9043bdc-9792-4ceb-a76f-d38d89531660" />

保存打包后的pck文件备用

之后选择该项来拆分原始的Buckshot Roulette.exe文件

<img width="1277" alt="image" src="https://github.com/user-attachments/assets/0f7ab735-0070-411f-8f6b-c417112db4ef" />

选择两次路径，第一次为Buckshot Roulette.exe的绝对路径，第二次为要输出的位置

现在你可以删除现在拆分后的pck文件了，然后将前面打包好的pck文件替换进来

之后将两个文件(Buckshot Roulette.exe和Buckshot Roulette.pck)放回游戏的根目录即可，注意两个文件都要重命名为Buckshot Roulette且必须将两个文件放在同一目录下

## 一点小问题

请使用Steam运行游戏，如果你直接点击exe文件来启动游戏将会导致邀请好友功能不可用
