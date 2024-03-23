# Cosmic-Reach-Wayland
Modified Linux GLFW Natives to force Cosmic Reach (and potentially other lwjgl3 applications) to run in a native Wayland window

This mod is potentially the first mod for Cosmic Reach (I'm just guessing, I haven't seen any others yet) and it makes the game run in a native Wayland window
I am a Linux user who has an Nvidia graphics card and Xwayland tends to have many rendering bugs when running Cosmic Reach so I compiled glfw-wayland for all the platforms Cosmic Reach supports and replaced libglfw.so with the glfw-wayland version and now the game runs in a native Wayland window!

## How to Install:
Extract CosmicReachWayland.zip and add the folder labled "linux" to the cosmic reach jar file using your archiving software. Works with both the linux and jar version of Cosmic Reach!
</br></br>This method should in theory work mostly the same for any lwjgl 3.5 compatible application as well

## Known Issues:
Significantly worse framerate. glfw-wayland is by no means a proper wayland implementation so the framerate is rather poor. It is a bit of a hacky solution, but it gets the job done for now. I'll update the description once a proper Wayland implementation is added
No window icon. Due to the implementation of glfw-wayland the window icon is the default Wayland icon and the command line logs errors about this. There is no way to fix this without modifying the source code and FinalForEach has made the game closed source and I want to respect his decision by not decompiling the game and uploading modified files

## Software Used:
glfw-wayland: [https://github.com/BoyOrigin/glfw-wayland](url)
</br>This project would not be possible without BoyOrigin's work on glfw-wayland
</br></br>glfw (duh): [https://github.com/glfw/glfw](url)
