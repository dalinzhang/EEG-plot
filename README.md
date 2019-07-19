# EEG-plot

## EEG montage plot

1. create montage object of EEG channels using MNE build-in montages

   Function description [here](https://martinos.org/mne/stable/generated/mne.channels.read_montage.html#mne.channels.read_montage)

```
montage = mne.channels.read_montage(kind='standard_1005')
```

The Montages can contain fiducial points in addition to electrode channels, e.g. biosemi64 contains 67 locations. In the following table, the number of channels and fiducials is given in parentheses in the description column (e.g. 64+3 means 64 channels and 3 fiducials).

Valid kind arguments are:

**Kind**                      Description

`standard_100`         Electrodes are named and positioned according to the international 10-05 system (343+3 locations)

`standard_102`        Electrodes are named and positioned according to the international 10-20 system (94+3 locations)

`standard_alphabeti`        Electrodes are named with LETTER-NUMBER combinations (A1, B2, F4, …) (65+3 locations)

`standard_postfixe`        Electrodes are named according to the international 10-20 system using postfixes for intermediate positions (100+3 locations)

`standard_prefixe`        Electrodes are named according to the international 10-20 system using prefixes for intermediate positions (74+3 locations)

`standard_prime`        Electrodes are named according to the international 10-20 system using prime marks (‘ and ‘’) for intermediate positions (100+3 locations)

`biosemi1`        BioSemi cap with 16 electrodes (16+3 locations)

`biosemi3`        BioSemi cap with 32 electrodes (32+3 locations)

`biosemi6`        BioSemi cap with 64 electrodes (64+3 locations)

`biosemi12`        BioSemi cap with 128 electrodes (128+3 locations)

`biosemi16`        BioSemi cap with 160 electrodes (160+3 locations)

`biosemi25`        BioSemi cap with 256 electrodes (256+3 locations)

`easycap-M`        EasyCap with 10-05 electrode names (74 locations)

`easycap-M1`        EasyCap with numbered electrodes (61 locations)

`EGI_25`        Geodesic Sensor Net (256 locations)

`GSN-HydroCel-3`        HydroCel Geodesic Sensor Net and Cz (33+3 locations)

`GSN-HydroCel-64_1.`        HydroCel Geodesic Sensor Net (64+3 locations)

`GSN-HydroCel-65_1.`        HydroCel Geodesic Sensor Net and Cz (65+3 locations)

`GSN-HydroCel-12`        HydroCel Geodesic Sensor Net (128+3 locations)

`GSN-HydroCel-12`        HydroCel Geodesic Sensor Net and Cz (129+3 locations)

`GSN-HydroCel-25`        HydroCel Geodesic Sensor Net (256+3 locations)

`GSN-HydroCel-25`        HydroCel Geodesic Sensor Net and Cz (257+3 locations)

`mgh6`        The (older) 60-channel cap used at MGH (60+3 locations)

`mgh7`        The (newer) 70-channel BrainVision cap used at MGH (70+3 locations)
