## Overview

This is a Fork of PsychoSmiley's LLM_Buttplug Extension for the text-generation-webui. The original extension makes linear actuators like the solace pro move in only short strokes, and the oscillation value makes it turn on and off in time with the oscillation value, which I find unfitting for a stroker like the solace. In this Fork an additional checkbox is added, to tell the program if you are using a linear actuator, if checked, the linear actuator will do constantly full strokes and the value given by the AI will determine how fast the stroker goes. Apart from that all original functions remain. I tested this with the Solace Pro, it might work for similar Toys with speed and stroke-depth settings.

## Original README by PsychoSmiley

This script will act as router between oobabooga/text-generation-webui and intiface-central server to move any type of linear and vibration sex toy.

## Installation

1. [Install oobabooga/text-generation-webui](https://github.com/oobabooga/text-generation-webui?tab=readme-ov-file#how-to-install), and download a model to run on it.
2. Execute depending of your os `cmd_windows.bat` or `cmd_{your os}` to activate the environment from text-generation-webui command prompt, and install requirement:

    ```cmd
    cd extensions
    git clone https://github.com/PsychoSmiley/LLM_Buttplug.git
    cd LLM_Buttplug
    pip install -r requirements.txt
    ```

3. Add `--extensions LLM_Buttplug` in `CMD_FLAGS.txt`.

4. Optional but recommended move the character template `templates\GPT-STROKER.json` to `characters` folder, to help json function calling. (tested with RP model `Athnete-13B-8bpw-h8-exl2`)

5. Download application https://intiface.com/desktop/ and run the server with toy ready.
 
6. Start oobabooga/text-generation-webui `start_windows.bat` (Select the character `GPT-STROKER.json`).

## Usage

1. If character output `stroke(1.0)` or `stroke(0.0)` it will move the sex toy to position `1.0` or `0.0` and oscillate.
