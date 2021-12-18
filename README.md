# Outer Wilds planet creation template
 A template project for adding planets to Outer Wilds with New Horizons.

<!-- TOC -->
- [Prerequisites](#prerequisites)
- [How to use this template](#how-to-use-this-template)
- [Beyond config files](#beyond-config-files)

<!-- /TOC -->

## Prerequisites
- Outer Wilds Mod Manager (get it from the [Outer Wilds Mods](https://outerwildsmods.com/) website)
- OWML installed in the Mod Manager
- A GitHub account (required for forking the repo and for releasing your mod to the public)

## How to use this template
1. Follow the instructions in [Outer Wilds New Horizons](https://github.com/xen-42/outer-wilds-new-horizons) on how to create planet config files. You can test them by putting them in the "planets" folder wherever New Horizons is installed.
2. Generate your repository from this template.
3. Clone your repository to your machine.
4. Edit `NewHorizonsTemplate/manifest.json`. See the "Editing manifest.json" section on the [Outer Wilds Mod Template](https://github.com/Raicuparta/ow-mod-template) repo for more info. Of note, do not change the filename "NewHorizonsTemplate.dll" and make sure to keep the dependencies line or it will not work.
5. Releasing the mod (see the "Relasing the mod" section on the  [Outer Wilds Mod Template](https://github.com/Raicuparta/ow-mod-template) repo for more info)

Note that if you want to stick exclusively to config files, you won't have to use Visual Studio or any other IDE or write any real code.

## Beyond config files
You can do more than just use config files with this. You can use the `INewHorizons` interface to create planets from a Dictionary (the dictionary will be arranged the same way the config files are) using `Create(Dictionary<string, object> config)` and then grab generated planets with `GetPlanet(string name)` and do whatever you want with them. 
