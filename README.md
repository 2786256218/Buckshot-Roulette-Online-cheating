# Procedure introduction
Download Godot PCK Explorer
https://github.com/DmitriySalnikov/GodotPCKExplorer/releases/download/1.5.3/GodotPCKExplorer_1.5.3_dotnet-ui-console-win-linux-mac.zip

Start by opening Godot PCK Explorer

<img width="1276" alt="image" src="https://github.com/user-attachments/assets/9b1cd5db-4617-4049-92ae-0a9cc90ebefd" />

Import Buckshot Roulette.exe into the tool

<img width="1277" alt="image" src="https://github.com/user-attachments/assets/44c95740-9bad-4c4c-9bc8-40c8155b9fdd" />

Select it

<img width="1277" alt="image" src="https://github.com/user-attachments/assets/75d84f12-9257-434b-8876-9585a6b46b75" />

Select an empty storage directory

Replace the downloaded MP_GameStateManager.gd file with ".\multiplayer\scripts\global scripts\MP_GameStateManager.gd"

After that, click the following option to select the unpacked directory in the modified file and repack it

<img width="1277" alt="image" src="https://github.com/user-attachments/assets/52dab4b9-47a1-4d57-9f42-6e121724b019" />

<img width="1277" alt="image" src="https://github.com/user-attachments/assets/b9043bdc-9792-4ceb-a76f-d38d89531660" />

Save the packaged PCK file in a directory for later use

Then select this item to split the original Buckshot Roulette.exe file

<img width="1277" alt="image" src="https://github.com/user-attachments/assets/0f7ab735-0070-411f-8f6b-c417112db4ef" />

Select twice, the first time for the exe file you want to split and the second time for the output directory. After splitting you will get an incomplete exe file and pck package

At this point, you can delete the split pck file and replace the previously packaged pck file. Note that the pck file and the exe file must be placed in the same directory, and both must be named Buckshot Roulette

At this point, the cheat function is implemented, just put the two binaries back in the root directory of the game

## A little trouble

The modified exe file needs to be launched with steam, and if you click on the exe directly to start, the invite friend function will become invalid
