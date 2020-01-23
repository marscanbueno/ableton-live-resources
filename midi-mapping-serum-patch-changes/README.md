# Midi Mapping Serum Patch Changes<a name="HOME"></a>

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Its been quite a struggle to figure out how exactly to midi map changing patches in serum running through ableton live using a midi controller online.  Since every link that i could find on the topic, simply led to another thread with no conclusive answer -- I am providing information on how I was able to accomplish this feat.

#### Please Note..

* This is one of many possible ways to handle Patch / Program Changes using Serum as VST within Ableton Live.  This happens to be the most convenient way for me.  Hope this helps you!

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

- [x] **GET** [Ableton Live](https://www.ableton.com)
- [x] **GET** [Serum](https://xferrecords.com/products/serum)
- [x] **GET** A Midi Controller (ie: a Midi Keyboard)
- [x] **GET** A Text Editor of your choice (ie: TextEdit, TextWrangler, BBEdit, Brackets, Notepad++, etc)


- [x] **KNOW WHAT YOU'RE GETTING INTO FIRST**
  - [x] View the ```serum.cfg``` file before edits:  [serum.cfg.bak](https://github.com/marscanbueno/ableton-live-resources/blob/master/midi-mapping-serum-patch-changes/Serum.cfg.bak)
  - [x] View the ```serum.cfg``` file after edits:  [serum.cfg](https://github.com/marscanbueno/ableton-live-resources/blob/master/midi-mapping-serum-patch-changes/Serum.cfg)


### Setup and Configuration<a name="setup"></a>

1. Provided you have Ableton Live and Serum pre-installed, navigate to the folder / directory that your ```serum.cfg``` preferences file is stored in.
2. Before editing ```serum.cfg``` make a duplicate / backup file.  Iʻve made a duplicate and renamed it ```serum.cfg.bak```.
3. Open ```serum.cfg``` in your text editor of choice.
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
6.  Open Ableton Live and insert a new instance of Serum onto a new Midi Channel.  Enjoy your mapped patch / preset selector!

### Usage<a name="usage"></a>

coming soon!

## Contributing<a name="contributing"></a>

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

## License<a name="license"></a>

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgements<a name="acknowledgements"></a>

..coming soon!

## Resources<a name="resources"></a>

..coming soon!