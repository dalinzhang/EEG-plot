# EEG-plot

## EEG montage plot

1. create montage object of EEG channels using MNE build-in montages

```
montage = mne.channels.read_montage(kind='standard_1005')
```

The Montages can contain fiducial points in addition to electrode channels, e.g. biosemi64 contains 67 locations. In the following table, the number of channels and fiducials is given in parentheses in the description column (e.g. 64+3 means 64 channels and 3 fiducials).

Valid kind arguments are:

`Kind`                       Description

`standard_1005`              Electrodes are named and positioned according to the international 10-05 system (343+3 locations)

standard_1020              Electrodes are named and positioned according to the international 10-20 system (94+3 locations)

standard_alphabetic        Electrodes are named with LETTER-NUMBER combinations (A1, B2, F4, …) (65+3 locations)

standard_postfixed         Electrodes are named according to the international 10-20 system using postfixes for intermediate positions (100+3 locations)

standard_prefixed          Electrodes are named according to the international 10-20 system using prefixes for intermediate positions (74+3 locations)

standard_primed            Electrodes are named according to the international 10-20 system using prime marks (‘ and ‘’) for intermediate positions (100+3 locations)

biosemi16                  BioSemi cap with 16 electrodes (16+3 locations)

biosemi32                  BioSemi cap with 32 electrodes (32+3 locations)

biosemi64                  BioSemi cap with 64 electrodes (64+3 locations)

biosemi128                 BioSemi cap with 128 electrodes (128+3 locations)

biosemi160                 BioSemi cap with 160 electrodes (160+3 locations)

biosemi256                 BioSemi cap with 256 electrodes (256+3 locations)

easycap-M1                 EasyCap with 10-05 electrode names (74 locations)

easycap-M10                EasyCap with numbered electrodes (61 locations)

EGI_256                    Geodesic Sensor Net (256 locations)

GSN-HydroCel-32            HydroCel Geodesic Sensor Net and Cz (33+3 locations)

GSN-HydroCel-64_1.0        HydroCel Geodesic Sensor Net (64+3 locations)

GSN-HydroCel-65_1.0        HydroCel Geodesic Sensor Net and Cz (65+3 locations)

GSN-HydroCel-128           HydroCel Geodesic Sensor Net (128+3 locations)

GSN-HydroCel-129           HydroCel Geodesic Sensor Net and Cz (129+3 locations)

GSN-HydroCel-256           HydroCel Geodesic Sensor Net (256+3 locations)

GSN-HydroCel-257           HydroCel Geodesic Sensor Net and Cz (257+3 locations)

mgh60                      The (older) 60-channel cap used at MGH (60+3 locations)

mgh70                      The (newer) 70-channel BrainVision cap used at MGH (70+3 locations)
