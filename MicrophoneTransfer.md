# Simple Microphone Transfer Characterization

## Tools
- Sound Source (like the [Manual Frequency and Intensity Calibrator](hardware/ManualfI.md))
- Sound Level Meter
- Computer with Audacity, Raven, Praat, or other audio software
- Computer with R

## Procedure
1. Place microphone of DUT and Sound Level Meter at the same distance from the sound source, right next to each other
2. Start recording on DUT
3. Set sound source to one frequency and amplitude
4. Wait a few seconds
5. Repeat steps 3 and 4 for several other frequencies and amplitudes
6. Turn off the sound source and sound level meter
8. Stop recording
9. Download sound file from DUT
10. Find the values of the various test sounds in LSBs or U
11. Create a sensitivity profile by graphing the output of the DUT with the frequency on the x axis, input amplitude from the sound level meter on the y axis, and the output of the DUT in LSBs or U on the z axis
12. Use `fit <- (z ~ x + y)` to create a calibration curve function for the DUT
