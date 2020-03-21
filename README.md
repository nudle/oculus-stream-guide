# oculus-stream-guide
### The LeahNudle guide to using the oculus mirror to stream vr games nicer :)

### SHORT VERSION BECAUSE I CANT STOP TYPING:
1. Install the oculus software, preferably on an SSD
2. Find your Oculus software directory
3. Find the Oculus Mirror exe, in `\Support\oculus-diagnostics\` from the base Oculus software directory
4. Download or create the .bat file with the stream settings in it
5. Put that .bat file in the Oculus Mirror Directory `<base Oculus directory>\Support\oculus-diagnostics\`

   Optional - Make a shortcut to that .bat file so you can run it from anywhere :)
   
6. Run the .bat file (or shortcut) and it'll open the Oculus Mirror with the correct settings
7. Capture that window in OBS as you would any other videogame

---

This might not be necessary for HL:Alyx because valve will probably make the preview you get outside of vr good for streaming but its really nice if you ever find a game that looks like poop in the desktop view (unity games are REAL bad for it)

When you install the oculus software to use the headset it'll install a tool in the `Support\oculus-diagnostics\` folder in the same directory as you install the software in (mine is my SSD `G:\Oculus\Support\oculus-diagnostics`) called `OculusMirror.exe`

this will mirror what you see in your headset, but as a separate exe so you can capture it better with OBS and configure it more. 

https://developer.oculus.com/documentation/native/pc/dg-compositor-mirror/ all the options are here, but I'll go over the ones I use in case you just want that.

i'll also upload the batch file i use, just chuck it in the same directory as OculusMirror.exe and it'll load the mirror up in 720p and with a higher fov than the default so it looks nice on the stream. doesn't affect your view or anything, just what is displayed on the mirror and therefore the stream. 

my batch file uses the setting `--RightEyeOnly` which means it'll show only what your right eye sees. This is important because you'll be physically closing your left eye when you aim (if you're right handed) so you wanna show people what you're aiming at.


depending on the eye you use to aim you might have to change the settings in the batch file. if you shoot left handed you'll probably aim with your left eye and should change the `--RightEyeOnly` to `--LeftEyeOnly` but if you're right handed/eyed just use `--RightEyeOnly`

if you run the  .bat file in the oculus mirror directory it'll open the oculus mirror in a window and you can capture that like you usually would in OBS, including putting your overlays and stuff over it. I use game capture but I'm sure whatever method you want would work. wouldn't recommend resizing the actual window but you can make it fit the screen in obs or whatever to make it fill the entire stream.

i also try and always have the actual game window in focus when i'm playing just in case it affects the framerate but i really don't know if you need to. Again i dunno if ANY of this will be necessary to stream half life alyx because I hope valve will know how to make a game streamable! but its still nice to get a unified streamable view for any VR game you might have issues with, especially unity games because theyre ALWAYS garbage because unity sucks.

if you can't download the file directly the settings are 

``start "" "OculusMirror.exe" --Size 1280 720 --FovTanAngleMultiplier 1.3 1.3 --DisableTimewarp --SymmetricFov --RightEyeOnly --DisableFovStencil --IncludeSystemGui --IncludeNotifications
exit``

put it in a text file in the same directory as oculusmirror.exe (mine is `G:\Oculus\Support\oculus-diagnostics\`) and rename it to streamMirror.bat

you can then make a shortcut to the bat file and run that from wherever you like to get the nice oculus mirror up for streams.

if you have questions i'm always down to try and help.

here's some previews if you wanna see the difference (game is 'Hotdogs, Horseshoes and Hand Grenades' on Steam which i highly recommend if you wanna mess around with vr guns)

# Using Oculus Mirror
![alt text](https://i.imgur.com/aRdZbZQ.png "Using Oculus Mirror")

# Not using Oculus Mirror
![alt text](https://i.imgur.com/54uBlSx.jpg " Not Using Oculus Mirror")

