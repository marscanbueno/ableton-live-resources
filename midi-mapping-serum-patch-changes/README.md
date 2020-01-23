![alt text](https://github.com/marscanbueno/ableton-live-resources/blob/master/midi-mapping-serum-patch-changes/midi-mapping-serum-patch-changes.png "Midi Mapping Serum Patch Changes")

# Midi Mapping Serum Patch Changes<a name="HOME"></a>

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Its been quite a struggle to figure out how exactly to midi map changing patches in [Serum](https://xferrecords.com/products/serum) running through [Ableton Live](https://www.ableton.com) using a midi controller on the web.  Since every link that i could find on the topic, simply led to another thread with no conclusive answer -- I am providing information on how I was able to accomplish this feat.

#### Please Note..

* This is one of many possible ways to handle Patch / Program Changes using [Serum](https://xferrecords.com/products/serum) as VST within [Ableton Live](https://www.ableton.com).  This happens to be the most convenient way for me based upon my production workflow.  I hope that this helps you!

## Table of Contents
* [Getting Started](#gettingstarted)
    * [Prerequisites](#prerequisites)
    * [Setup & Configuration](#setup)
    * [Usage](#usage)
* [License](#license)
* [Acknowledgements](#acknowledgements)
* [Resources](#resources)

## Getting Started<a name="gettingstarted"></a>

### Prerequisites<a name="prerequisites"></a>

- [x] **SOFTWARE / HARDWARE**
  - [x] **GET** [Ableton Live](https://www.ableton.com)
  - [x] **GET** [Serum](https://xferrecords.com/products/serum)
  - [x] **GET** A Midi Controller (ie: a Midi Keyboard)
  - [x] **GET** A Text Editor of your choice (ie: TextEdit, TextWrangler, BBEdit, Brackets, Notepad++, etc)
  - [x] **GET** The CC or Note values that you desire to use for midi mapping your controller


- [x] **SKILLS REQUIRED**
  - [x] Navigating your file system
  - [x] Duplicating files
  - [x] Renaming files
  - [x] Editing files

- [x] **KNOW WHAT YOU'RE GETTING INTO FIRST**
  - [x] View the ```serum.cfg``` file before edits:  [serum.cfg.bak](https://github.com/marscanbueno/ableton-live-resources/blob/master/midi-mapping-serum-patch-changes/Serum.cfg.bak)
  - [x] View the ```serum.cfg``` file after edits:  [serum.cfg](https://github.com/marscanbueno/ableton-live-resources/blob/master/midi-mapping-serum-patch-changes/Serum.cfg)


### Setup and Configuration<a name="setup"></a>

1. Provided you have [Ableton Live](https://www.ableton.com) and [Serum](https://xferrecords.com/products/serum) pre-installed, navigate to the folder / directory that your ```serum.cfg``` preferences file is stored in.
  * ```serum.cfg``` is located in the following folder / directory depending on what operating system you are using:
    * **[MacOS]**:  ```~/Library/Preferences/Serum.cfg```
    * **[WindowsOS]**:  ```%APPDATA%/Xfer/Serum```
2. Before editing ```serum.cfg``` make a duplicate / backup file.  Iʻve made a duplicate and renamed it ```serum.cfg.bak```.  Feel free to name your backup whatever you want that will identify it to you as a backup.

3. Open ```serum.cfg``` in your text editor of choice.  My flavor of the month is [Brackets](http://brackets.io)!

4. We will now edit a few lines within ```serum.cfg``` to allow us to change presets using buttons on our hardware device.  We will need to know if we will be using buttons that transmit Midi CCs or Notes, and what their values are.  In the following example, I will use Midi CCs.
  1. Line 33:  replace ```X``` with ```1```.  
  
      * where it said:
  
      ```[X] enable/disable this section (1 for CC, 2 for NOTES)```
        
      * it should now read:
  
      ```[1] enable/disable this section (1 for CC, 2 for NOTES)```
      
  2. Line 34:  replace both of the ```X```'s with the desired CCs for your controller.  in this example i use ```34``` for my previous patch / preset, and ```35``` for next patch / preset.  substitute ```34``` and ```35``` with the values that are specific to your controller.
  
      * where it said:
      
      ```[X][X] (increment / decrement CC for Preset Changes)```

      * it should now read:

      ```[35][34] (increment / decrement CC for Preset Changes)```
  
5. Save your changes!
6.  Open [Ableton Live](https://www.ableton.com) and insert a new instance of [Serum](https://xferrecords.com/products/serum) onto a new Midi Channel.  Enjoy your mapped patch / preset selector!

## License<a name="license"></a>

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgements<a name="acknowledgements"></a>

Rez, [Adlib Beats](https://soundcloud.com/ad-lib-beats), and [Beat Le Juice](https://soundcloud.com/beatlejuicemusic) all inspired me to post up this information!  If you found this information useful, look them up on Soundcloud and give them a follow in appreciation!

## Resources<a name="resources"></a>

..coming soon!