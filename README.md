# Description
Project Dialogue Expanded is, as the name suggests, a mod for the game Chef RPG that adds lines of dialogue for the main characters in game.

**Currently** the game adds lines for **Uriel** and **Alloys**

The mod works by injecting 71 new lines to the base game through the patching of the methods related to translation 
and new relationship level chains of decisions, to allow the inclusion of dialogues with player input. It currently
supports the build *25090380* (Tidehaven update). This way, it should be compatible with any other mod that doesn't change
lines of dialogue.

**Disclaimer - AI usage**
Since this is my first ever mod, and the first time I work with C#, LLM models were used for support with coding and debugging. 
This usage, however, didn't extend to any of the dialogue added to the game. 

# Future projects:
I built the patches in a way that makes possible to future add-ons to other NPCs dialogue pool. So I should be able to release new 
versions of this mod for other characters in the near future, although this is a side project and I don't commit to a timeline. ~~Also, 
you may notice the new lines won't be accompanied by portrait emotions. This is a known issue, and it's my top priority to fix it in 
the next version.~~ (fixed)

That said, the game in it's currently state only supports up to 10 lines of dialogue for relationship level. So I intend to tinker with
the game modules to find a way to increase this limit in the medium-term.  

# Compile

Although the source code is available, I wouldn't recommend the compilation from it if you don't know what you're doing. That said,
if you want to compile the mod from the source code, you just need to follow the BepInEx documentation found in this link: https://docs.bepinex.dev/articles/dev_guide/plugin_tutorial/2_plugin_start.html 

# Install

This mod needs the following dependencies to work:
- BepInEx (5.4.23.5), which can be found in: https://github.com/BepInEx/BepInEx
  - Download the 5.4.23.5 release for your OS and follow installation instructions.
      - If you're running the game on Linux with a compatibility layer (Ex.: Proton), you should follow the windows instruction and add "WINEDLLOVERRIDES="winhttp=n,b" %command%" to the game launch option.

After BepInEx is properly installed and launched (you should have the path "~/Chef RPG/BepInEx/plugins/" if everything went well),
just extract the zip file content to the folder "plugins" and start the game. 

## Uninstall
This mod shouldn't cause any problem to uninstall. Just delete the mod folder and you're good to go. 
