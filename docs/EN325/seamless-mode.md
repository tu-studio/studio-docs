# E-N 325 Seamless Mode

## Important

- Turn off the WFS-Panels when leaving
- Make sure the power is turned off (power key 0) when leaving the studio
- Leave the place tidy (e.g. move table back, move chairs to the back)

## Quickguide Seamless System

1. Turn the power key to I (beside the door)
2. Plugin USB-MADIface
    - Options -> Reset Mix -> Straight Playback (when connected the first time)
    - Outputfader can be linked to create a "masterfader"
3. In the machineroom turn on
    - Riviera: OscRouter, Ambisonics, WFS 1-64
    - Wintermute: WFS 65-192
    - Taunus: Dante-Madi Conversion
4. In the machineroom set MADI-Bridge
    - Out 8 <- In 7 (Madiface Direct)
    - Out 8 <- In 1 (seamless mode)
5. Turn on
    - Ambisonics speaker with switch besides the door
    - WFS-Panels with switches under the Dante-Network switch
6. The seamless system is controled via OSC e.g. with the seamless plugins
    - ip-address: xxx.xxx.xxx.24
    - port (oscrouter): 4455
    - port (reverb/master): 57120
7. play audio through madiface
    - 1-32 Sources
    - 33-36 Ambisonics 1st Order
    - 37-52 Ambisonics 3rd Order
    - 53 LFE direct
