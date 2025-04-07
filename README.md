# Left 4 Dead 2 Autoexec

My own Personal Autoexec i worked on for the past Years.</br>
Each Category and Command has an explanation and is easily customizable or is expandable by executing your own Config.

## Usage
Download the Repository as .zip and extract the autoexec.cfg and configs folder into left4dead2\cfg, default path is:</br>
```
"C:\Steam\steamapps\common\Left 4 Dead 2\left4dead2\cfg"
```

## Start Options
Go to Steam Libary, rightclick Left 4 Dead 2, click Properties, "Set Launch Options" and paste the ones you wanna use there seperated by a space.

```
// Removes the Motion Blur when shader effects on high or above (recommended)
+mat_motion_blur_percent_of_screen_max 0

// Set to 0 for no HDR, 1 for LDR+bloom on HDR maps, and 2 for full HDR on HDR maps (0 is basically fullbright, some servers might block it)
+mat_hdr_level 0

// When loading a game with this parameter, the intro video will not play (recommended)
-novid

// Disables joystick support
-nojoy

// Disables Steam controller system
-nosteamcontroller

// Starts the game with the developer console enabled (recommended)
-console

// Sets the game language to the one specified. Examples: en (English), da (Danish), nl (Dutch), fi (Finnish), fr (French), de (German), it (Italian), ja (Japanese), ko (Korean), no (Norwegian), pl (Polish), pt (Portuguese), ru (Russian), zh-CN (Simplified Chinese), zh-TW (Traditional Chinese), es (Spanish), sv (Swedish), hu (Hungarian), tr (Turkish), bg (Bulgarian), cs (Czech), el (Greek), pt-BR (Portuguese - Brazil), ro (Romanian), es-419 (Spanish - Latin American, th (Thai), uk (Ukrainian), vn (Vietnamese)
-language <country code>

// Disables Gore (recommended)
-lv

// Disables IPX Support (recommended)
-noipx

// Disable SourceTV (recommended)
-nohltv

// Sets the game's priority to High (worth to test if bad performance)
-high

// Precaches all Survivors
+precache_all_survivors 1

// Host game client port (may fixes issues with "Failed after 10 retrys" Messages)
+clientport 27619

// Forces the engine to use operating system mouse parameters (recommended)
-noforcemparms

// Forces the engine to use operating system mouse acceleration (recommended)
-noforcemaccel

// Translation Layer to switch the Renderer Backend to Vulkan (recommended, can improve performance and latency)
-vulkan

// Number of threads to allocate for the thread pool, default is 3 (recommended setting to half the available threads)
-threads <value>

// Forces specific Refresh rate (recommended when you have issues with your refresh rate)
-refresh <value>
```

## Recommended Video Settings
My recommended Video Settings for Performance / Latency.

### Aspect Ratio
- Set to your desired Aspect Ratio

### Resolution
- Set to your Screens Resolution, you may lower it if you are playing on a weak system

### Display Mode
- Fullscreen for best performance / latency

### Film Grain Amount
- None

### Anti-Aliasing Mode
- Off

### Filtering Mode
- Anisotropic 16x

#### Wait for Vertical Sync
- Off for best performance / latency

### Shader Detail
- Low

### Effect Detail
- High (Lower Values affect the Tank Rock, making it pop in if thrown from further away)

### Model / Texture Detail
- Low

### Multicore Rendering
- Enabled (expreiment turning it off if bad performance)

### Paged Pool Memory Available
- High (expreiment turning it off if bad performance)



## Add your own Config

If you wanna add your own config you can easily do so by placing your config file in the left4dead2\cfg folder and adding it to the autoexec.

```
// Other Configs //

exec promode

or

exec config\promode

for a subfolder
```
