# minecraft-lwjgl-macos

## why
By default minecraft uses lwjgl 3.2.2 which is not compatible with macos on aarch64 (M1).
this also includes a older verison of openal which does not support device enumeration on macos.

this repository allows you to update to the latest lwjgl 3.3.0 and/or a unreleased version of openal.
this will allow correct playback device names to be used on macos.
and the use of minecraft on a m1 device without rosetta.

## how

Step 1:
Install MultiMC5
Step 2:
Install Java

M1 devices: https://www.azul.com/downloads/?os=macos&architecture=arm-64-bit&package=jre
Intel devices: https://www.azul.com/downloads/?os=macos&architecture=x86-64-bit&package=jre

Java 17 is required for minecraft 1.18

Step 3:
Create a new MultiMC profile

Step 3.5:
IMPORTANT:
If you are planning to install Fabric/Forge you need to install it now. or it will break


Step 4:
In the version tab of MultiMC select LJGL 3.2.2 and click customize
then click on the edit button
replace the file it opens with one of the following

M1 devices: [lwjgl-3.3.0-aarch64.json](lwjgl-3.3.0-aarch64.json)
Intel devices: [lwjgl-3.3.0-X86-64.json](lwjgl-3.3.0-X86-64.json)

Step 5:

Launch the game
