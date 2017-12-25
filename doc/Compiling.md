* [Windows](#windows)
  * [Setting up your build environment](#setting-up-your-build-environment)
  * [Compiling the game](#compiling-the-game)

## Windows
### Setting up your build environment

1)	Download the 32-bit version of the Lazarus IDE from the [Lazarus website](http://www.lazarus-ide.org/). Using the 64-bit version is possible, but that won't be covered in this guide.
2)	Install Lazarus to a folder of your choosing.
3)	Create a folder. I will refer to this folder as 'DoomProject', for the purposes of this guide. 
4)	Download the DoomRL high quality and low quality .zip files from the [DoomRL website](http://drl.chaosforge.org/). Extract the .zip files into DoomProject. I'll refer to these folders as DoomGameHQ and DoomGameLQ.
5)	Download DoomRL source files .zip from GitHub by clicking the 'Clone or download' button, and choosing 'Download Zip'. Extract the .zip folder into DoomProject. I'll refer to this folder as SourceCode.
6)	Download the [fpcvalkyrie source files .zip](https://github.com/ChaosForge/fpcvalkyrie/) in the same way. Extract to DoomProject.
7)	**Make sure that the fpcvalkyrie folder name is 'fpcvalkyrie'**. This is important, because the DoomRL source code is configured to use that name, specifically.
8)	Copy all .DLL files from DoomGameHQ to SourceCode\bin.
9)	Copy the DoomGameHQ\mp3 and DoomGameHQ\wavhq folders to SourceCode\bin.
10)	Copy the DoomGameLQ\music and DoomGameLQ\wav folders to SourceCode\bin.
11)	Create a folder named 'tmp' in SourceCode.
12)	[Optional] Rename SourceCode\bin\config.lua to configlq.lua and SourceCode\bin\confighq.lua to SourceCode\bin\config.lua. The GitHub repository uses the low quality audio, by default. This step allows DoomRL to run with the HQ audio files.

At this point, your folder structure should look like this. I've included only the first two subfolders of the folders in DoomProject:
* DoomProject
  * DoomGameHQ
      * backup
      * modules
  * DoomGameLQ
      * backup
      * modules
  * SourceCode
      * bin
      * mp3
  * fpcvalkyrie
      * libs
      * lua

### Compiling the game
1)	Open SourceCode\src\makewad.lpi in Lazarus and select 'Build' in the Run menu. If you are prompted to create the missing 'tmp' directory, hit the 'Create' button.
2)	Navigate to SourceCode\bin folder and run makewad.exe. If it runs correctly, you should now see doomrl.wad and core.wad in the SourceCode\bin folder.
3)	Open SourceCode\src\doomrl.lpi in Lazarus, and click Build
4)	Run doomrl.exe in the SourceCode\bin folder to play the game.
