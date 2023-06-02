# :ice_cube: Filtering Noise from Ice Sheets using Dynamic Bandstop Filters :ice_cube:

<h1> Team Members </h1>
- Naomi Mo <br>
- Didi Kamalova <br>
- Caleb Matthews <br>
- Anabella Hernandez <br>

<h1> Results </h1>
In order to maximize our SNR, we combined our most successful filters, in order to eliminate the parabola-esque curve, as well as the eye patches. To achieve this, we added our three-segment parabolic-arc bandstop filter and our time-triggered eyepatch bandstop filter together in the iterator. We ran each segment of data first through the parabolic bandstop and then through the eyepatch filter (if active) before moving to the next time slice. This methodology proved very effective, yielding an SNR of 36.20 dB. <br>

By adding further optimizations, such as additional bandstop filters across certain frequencies with higher spectral density (an example if shown in figure 14), as well as experimenting with elliptic filters with extremely high stop band attenuation, we achieved an even higher SNR: 36.36 dB.

<p align="center">
  <img src="media/final_spectrogram.png" title="Final Spectrogram" width = "500">
</p>
<p align="center">
  <img src="media/final_radargram.png" title="Final Radargram" width = "500">
</p>
