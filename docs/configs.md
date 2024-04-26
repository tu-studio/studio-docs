# Config Files
## Speaker Positions
??? info "About the coordinate formats"
    Speaker Positions for the studios are supplied both in cartesian and in spherical coordinate systems.
    #### Cartesian:
    the y axis points in the viewing direction when sitting in the center of the room and looking at speaker 1, the x axis points to the right.
    #### Spherical:
    *azimuth/elevation/distance* coordinates are given in degrees. azimuth =0° points in the viewing direction when sitting in the center of the room and looking at speaker. Azimuth increases counter-clockwise. The ceiling speaker is at elevation =90°

- Small Studio Dome [xyz](configs/small_studio_speakers_xyz.csv){:download="speakerpositions_small_studio_xyz.csv"}/[aed](configs/small_studio_speakers_aed.csv){:download="speakerpositions_small_studio_aed.csv"}
- Large Studio Dome: [xyz](configs/large_studio_speakers_xyz.csv){:download="speakerpositions_large_studio_xyz.csv"}/[aed](configs/large_studio_speakers_aed.csv){:download="speakerpositions_large_studio_aed.csv"}
    - coordinate origin is set below the ceiling speaker, 1.13m above the ground


## IEM Decoder

The following configs are needed to use the [IEM Plugin Suite](https://plugins.iem.at/) in the studios:

- [Large Studio Dome](configs/large_studio_dome.json){:download="large_studio_dome.json"}
- [Small Studio Dome](configs/small_studio_dome.json){:download="small_studio_dome.json"}
- [Small Studio Ring](configs/small_studio_8ring.json){:download="small_studio_ring.json"}
??? info "How to load configs for the IEM plugins"
    1. start your desired decoder (eg. the AllRADecoder)
    2. press import
    3. select your config file
    4. in the section "Calculate Decoder" set the Decoder order to your desired order
    5. press "Calculate Decoder"
    6. when using the AllRADecoder, place a distanceCompensator in the effect chain after the decoder
    7. import the same config file there

## TotalMix Workspaces

These workspaces are used to control the MADIface USB in the small studio:

- [EN325 Direct Mode](configs/tu_studio_EN325_direct.tmws){:download="tu_studio_EN325_direct.tmws"}
- [EN325 Seamless Mode](configs/tu_studio_EN325_seamless.tmws){:download="tu_studio_EN325_seamless.tmws"}

??? info "How to load a TotalMix Workspace"
    1. Open TotalMix FX
    2. Click on the "File" button (top left)
    3. Click on "Load Workspace"
    4. Select the workspace file

## Reaper Template Projects
These projects require the IEM Plugins and have a preset channel assignment for working in the studios:

- [EN324 Template Project](configs/en324_reaper_template.RPP){:download="en324_reaper_template.RPP"}

If Reaper complains about the plugins not being available simply replace the missing plugins with your installed copies, and import the correct config files in the AllRADecoder and the DistanceCompensator.

To use the binaural decoder mute the main decoder channel and unmute the binaural decoder.