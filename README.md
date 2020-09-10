# Noise-Reduction

### Course project at Faculty of Mathematics - University of Belgrade.

Goal is to remove "White noise" from given audio sample and sample of white noise.
This is implementation inspired by [Audacity algorithm](https://wiki.audacityteam.org/wiki/How_Audacity_Noise_Reduction_Works).
[C++ code](https://github.com/audacity/audacity/blob/master/src/effects/NoiseReduction.cpp).

#### Steps:
    
    - Calculate STFT with window over noise
    - Calculate mean and std in db over noise
    - Create mask based on statistics
    - Calculate STFT over audio
    - Apply mask on audio
    - Recover signal using ISTFT
    - And FFT over whole signal
    - Applying window function
    - Finally, IFFT for final signal


