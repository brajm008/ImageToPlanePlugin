# Image To Plane Plugin

This is a plugin for TaleSpire using BepInEx.

## Install

Go to the releases folder and download the latest and extract to the contents of your TaleSpire game folder.

## Usage

After installing, you can press F1 to bring up a dialog to select an image.
Upon selecting an image, a plane the with selected image will be displayed.
Pressing F1 will allow to select a new image.
Pressing F2 will clear the map of the displayed image.
The plane currently has no networking so it is only visible locally.
The plane scales the image to currently render at 40px per tile.
You can change the bind keys in config editor.

## How to Compile / Modify

Open ```ImageToPlanePlugin.sln``` in Visual Studio.

You will need to add references to:

```
* BepInEx.dll  (Download from the BepInEx project.)
* Bouncyrock.TaleSpire.Runtime (found in Steam\steamapps\common\TaleSpire\TaleSpire_Data\Managed)
* UnityEngine.dll
* UnityEngine.CoreModule.dll
* UnityEngine.InputLegacyModule.dll 
* UnityEngine.UI
* Unity.TextMeshPro
* System.Windows.Forms
```

Build the project.

Browse to the newly created ```bin/Debug``` or ```bin/Release``` folders and copy the ```ImageToPlanePlugin.dll``` to ```Steam\steamapps\common\TaleSpire\BepInEx\plugins```