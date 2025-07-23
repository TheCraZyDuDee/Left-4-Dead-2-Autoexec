## Launch Arguments
Moved here to reduce clutter at the main readme.<br>
Note: Many of them are not fully tested but are listed in the Developer Community Wiki found [here](https://developer.valvesoftware.com/wiki/List_of_Left_4_Dead_2_console_commands_and_variables)

Go to Steam Libary, rightclick Left 4 Dead 2, click Properties, "Set Launch Options" and paste the ones you wanna use there seperated by a space.

### General
```
// When loading a game with this parameter, the intro video will not play (recommended)
-novid

// Starts the game with the developer console enabled (recommended)
-console

// Sets the game's priority to High (worth to test if bad performance)
-high

// Number of threads to allocate for the thread pool, default is 3 (recommended leaving at least one thread for the system, can improve performance)
-threads <value>

// Forces specific Refresh rate (recommended when you have issues with your refresh rate)
-refresh <value>

// Translation Layer to switch the Renderer Backend to Vulkan (recommended, can improve performance and latency tough i would recommend manually installing dxvk)
-vulkan

// Sets the game language to the one specified. Examples: en (English), da (Danish), nl (Dutch), fi (Finnish), fr (French), de (German), it (Italian), ja (Japanese), ko (Korean), no (Norwegian), pl (Polish), pt (Portuguese), ru (Russian), zh-CN (Simplified Chinese), zh-TW (Traditional Chinese), es (Spanish), sv (Swedish), hu (Hungarian), tr (Turkish), bg (Bulgarian), cs (Czech), el (Greek), pt-BR (Portuguese - Brazil), ro (Romanian), es-419 (Spanish - Latin American, th (Thai), uk (Ukrainian), vn (Vietnamese)
-language <country code>

// Disables joystick support
-nojoy

// Disables Steam controller system
-nosteamcontroller

// Disables IPX Support (recommended)
-noipx

// Disable SourceTV (recommended)
-nohltv

// Forces the engine to use operating system mouse parameters (recommended)
-noforcemparms

// Forces the engine to use operating system mouse acceleration (recommended)
-noforcemaccel

// Precaches all Survivors
+precache_all_survivors 1

// Host game client port (may fixes issues with "Failed after 10 retrys" Messages)
+clientport 27619
```

### Visuals & Performance
#### Confirmed Working
```
// Removes the Motion Blur when shader effects on high or above (recommended)
+mat_motion_blur_enabled 0
+mat_motion_blur_percent_of_screen_max 0

// Set to 0 for no HDR, 1 for LDR+bloom on HDR maps, and 2 for full HDR on HDR maps (0 is basically fullbright, some servers might block it)
+mat_hdr_level 0

// Disables post-processing color correction LUTs (makes the game look "flat")
+mat_colorcorrection 0

// Disables Texture blending
+mat_disable_fancy_blending 1

// Disables Gore (recommended)
-lv
```
#### Unconfirmed (need testing)
```
// Disables rendering of real-time Shadows
+r_shadows 0
+cl_player_shadow_dist 0

// Disables Bloom
+mat_disable_bloom 1
+mat_bloomscale 0

// Disables Depth of Field
+mat_dof_enabled 0

// Disables 3D sky boxes
+r_3dsky 0

// Disable dynamic lighting
+r_dynamic 0

// Disables Vingette (darkening arround screen corners)
+mat_vignette_enable 0

// Disables footstep particles
+cl_footstep_fx 0
```

### Miscellaneous (unconfirmed, need testing)

```
// Smoothes the stairs, disabling makes the stairs bumpy
+smoothstairs 1

// Disables Viewbobbing (recommended tough it's personal preference)
+cl_viewbob 0
```