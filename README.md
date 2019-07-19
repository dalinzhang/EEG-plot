# EEG-plot

## EEG montage plot

1. create montage object of EEG channels using MNE build-in montages

   Function description [here](https://martinos.org/mne/stable/generated/mne.channels.read_montage.html#mne.channels.read_montage)

   ```
   montage = mne.channels.read_montage(kind='standard_1005')
   ```
   
   The Montages can contain fiducial points in addition to electrode channels, e.g. biosemi64 contains 67 locations. In the following table, the number of channels and fiducials is given in parentheses in the description column (e.g. 64+3 means 64 channels and 3 fiducials). The 3 fiducials are 'Nz', 'LPA' and 'RPA'.
   
   Valid kind arguments are [here](https://martinos.org/mne/stable/generated/mne.channels.read_montage.html#mne.channels.read_montage)

2. 2d/3d montage plot

   Function description [here](https://martinos.org/mne/stable/generated/mne.channels.Montage.html#mne.channels.Montage)
   
   **2d plot**
   
   ```
   montage.plot(kind='topmap')
   ```
   
   **3d plot**
      
   ```
   montage.plot(kind='3d')
   ```

3. 
