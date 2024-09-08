**Reverb Audio Plugin**

**Overview**
This is a reverb audio plugin developed using the JUCE framework. The plugin applies various reverb effects, allowing users to customize the sound with a variety of sliders and options. It also supports Impulse Response (IR) files for setting reverb characteristics, giving users even more flexibility in shaping their sound.

**Features**
Cut-Off Slider: Controls the cutoff frequency for the reverb filter.
Rate Slider: Adjusts the rate of modulation within the reverb.
Depth Slider: Controls the depth of modulation.
Gain Slider: Adjusts the overall gain level of the reverb effect.
Filter Menu: Choose different filter types to apply to the reverb.
Phaser Menu: Select from multiple phaser options to add a phaser effect to the reverb.
Wet/Dry Mix:
Wet Slider: Controls the level of the reverb effect in the mix.
Dry Slider: Controls the level of the original dry signal.
Room Slider: Adjusts the simulated room size for the reverb effect.
Width Slider: Sets the stereo width of the reverb effect.
Damping Slider: Controls how much high-frequency damping is applied.
IR Length Slider: Adjusts the length of the Impulse Response (IR) for reverb customization.
Type of Reverb Menu: Choose between different reverb types (e.g., Hall, Plate, Room, etc.).
File Choice Button: Allows users to upload their own Impulse Response (IR) file to shape the reverb effect.
Files Included
PluginProcessor.cpp
PluginEditor.cpp
PluginProcessor.h
PluginEditor.h
DSPDelayLineTutorial.h
ReverbPlugin.jucer
These files contain the source code and project configuration necessary to build and run the plugin.

**Installation & Usage**

**Building the Plugin (macOS - AU)**
Prerequisites:

JUCE Framework: Download JUCE from JUCE's official website.
Xcode: Install Xcode from the Mac App Store to compile the project.
Steps:

Clone the Repository:
bash:

git clone https://github.com/<matthewmforget>/<Reverb-Plugin>.git

Open in Projucer:
Open Projucer from your JUCE installation.
Load the .jucer file by clicking Open Existing Project and navigating to ReverbPlugin.jucer.
Make sure AU (Audio Unit) is enabled under Plugin Formats in the project settings.
Open in Xcode:
In Projucer, click Save Project and Open in IDE. This will generate Xcode project files and open them in Xcode.
Build in Xcode:
In Xcode, select the Audio Unit target from the scheme dropdown.
Hit Cmd + R or click Run to build the plugin.
Once the build is complete, you will find the .component file in the build folder.
Install the Plugin:
Copy the generated .component file to your Audio Unit plugin folder:
bash:

/Library/Audio/Plug-Ins/Components
Use the Plugin:
Open your DAW (e.g., Logic Pro, Ableton Live).
Rescan your plugins if needed, and insert the reverb plugin on an audio track. Adjust the sliders and combo boxes to customize the reverb, and upload your own IR file to create a unique reverb profile.
Plugin Controls
Sliders

Cut-Off Slider: Controls the cutoff frequency, shaping the tonal quality of the reverb.
Rate Slider: Adjusts the modulation rate for creative effects.
Depth Slider: Controls the modulation depth, altering the intensity of the reverb's modulation.
Gain Slider: Adjusts the overall loudness of the reverb effect.
Wet Slider: Sets the level of the reverb effect (processed signal).
Dry Slider: Sets the level of the original audio (unprocessed signal).
Room Slider: Adjusts the room size simulation, affecting how spacious the reverb sounds.
Width Slider: Controls the stereo spread of the reverb effect.
Damping Slider: Adds high-frequency damping to simulate absorption of sound in a physical space.
IR Length Slider: Determines the duration of the reverb tail when using IR files.
Combo Boxes

Filter Menu: Choose a filter type to alter the tonal characteristics of the reverb.
Phaser Menu: Apply different phaser effects to the reverb, for a more dynamic and evolving sound.
Type of Reverb Menu: Select between different reverb types (e.g., Hall, Plate, Room).
IR File Option

File Choice Button: Select an external Impulse Response (IR) file to shape the reverb effect, allowing for a custom reverb environment.
