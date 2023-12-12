# E-N 325 Seamless Mode

!!! warning "Important"   
    - Turn off the WFS-Panels and ALL speakers when leaving!
    - Make sure the power is turned off (power key 0) when leaving the studio
    - Leave the place tidy (e.g. move table back, move chairs to the back)

## First Steps
1. Connect your Computer to the interface (MADIface USB)
2. Turn the power key to I (beside the door)
3. *(if not already installed)* Install [drivers](https://www.rme-audio.de/de_madiface-usb.html) for the MADIface (not the firmware update)

## User Guide Seamless Mode
1. Download correct TotalMix config [here](../configs.md) and import it into TotalMix
2. Make sure all Fadergroups are turned down
3. In the machineroom:
    1. Set MADI-Bridge to preset 2
    2. Hold the *recall* button to load the preset (not the *store* button!)
        <!-- TODO insert foto -->
    3. Turn on the rendering servers:
        - Riviera: OscRouter, Ambisonics, WFS 1-64
        - Wintermute: WFS 65-192

4. Turn on
    - Ambisonics speakers with switch besides the door
    - WFS-Panels with switches under the Dante-Network switch
5. *(if not already installed)* Download the [Seamless Plugin Suite](https://github.com/TU-Studio/seamless-plugin-suite/releases/latest) for your Operating System
    1. Extract the Zip file
    2. Move the VST3 to your system VST3 folder or use the standalone Plugins

6. The seamless system is controled via OSC with the seamless plugins – first configurte the main plugin:
    - Set the OSC Send Adress to the Address of the OSC-Router
    - Ip-address: xxx.xxx.xxx.24
    - Port (oscrouter): 4455

7. Play audio through the madiface

    | Channels | Seamless Mapping |
    | ---- | ---- |
    | 1-32 | Sources |
    | 33-36 | Ambisonics 1st Order |
    | 37-52 | Ambisonics 3rd Order |
    | 53 | LFE direct |

8. Use a client plugin on each track to contol the gain of the HOA and WFS System as well as the position of the source
    - Set the Source Index to the channel number of the source
    - Set the HOA Gain to the desired gain of the HOA System
    - Set the WFS Gain to the desired gain of the WFS System
    - Position the source

9. When Leaving:
    - turn off the WFS-Panels and ALL speakers
    - turn off the power using the power key (set to 0)
    - leave the space tidy
