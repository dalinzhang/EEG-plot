# EEG-plot

## EEG montage plot

1. create montage object of EEG channels using MNE build-in montages

   Function description [here](https://martinos.org/mne/stable/generated/mne.channels.read_montage.html#mne.channels.read_montage)

   ```
   montage = mne.channels.read_montage(kind='standard_1005')
   ```
   
   The Montages can contain fiducial points in addition to electrode channels, e.g. biosemi64 contains 67 locations. In the following table, the number of channels and fiducials is given in parentheses in the description column (e.g. 64+3 means 64 channels and 3 fiducials).
   
   Valid kind arguments are [here]
