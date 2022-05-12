# E-N 325 Octa Mode

## Important
- Make sure the power is turned off (power key 0) when leaving the studio
- Leave the place tidy (e.g. move table back, move chairs to the back)

## Quickguide Octachannel System
1. Turn the power key to I (beside the door)
2. Plugin the USB-Cable from the AudioInterface (Scarlett 18i20, 1st Gen)
    - The audio device is class compliant and can therefore used by linux (and in theory mac) users without driver
    - Windows and Mac User can download a [driver and control application here](https://downloads.focusrite.com/focusrite/scarlett-1st-gen/scarlett-18i20-1st-gen)
    - The application is not M1-mac compatible (s. troubleshooting)
3. Turn on the speakers by pressing "Lautsprecher 1" and "Lautsprecher 2" on the control terminal
    - The HEDD speaker were on channel 1-8
    - The Subwoofers were on channel 9-10
4. **Do not change the internal routing of the interface**


### Troubleshooting
- After installing the driver it asks for firmware update
    - Yes do it.
    - Update fails or similiar?
        - try the older or newer version of the driver from focusrite.
- The interface does not appear on my system
    - Turn it off, disconnect USB, turn it on, plug in USB
- The interface is connected but I don't hear anything
    - Make sure the internal routing is set correctly
        - Use alsamixer in linux
        - Use Scarlett Mixcontrol
- Apple-M1 User: in generally the interface works but you are not able to control the internal settings. If running into problems with software not playing back on all channels try to change the number of input/output channels in Apples "Audio MIDI Setup". 
- I don't hear anything. Make sure...
    - the speaker are turned on (HEDD speaker should have a small green LED on the front)
    - in your audio-software/systemsetting the right device is set
    - in Alsamixer/ScarlettMixcontrol the routing is right
    - the Master Volume(s) are not muted/set to 0 in alsamixer.
    - the Hardware Volume knob at the interface itself is turned full to the right.
