# BLOOD VOLUME FLOW ANALYSIS USING DOPPLER ULTRASOUND SCAN

Doppler Ultrasound is a non-invasive method used to image tissue and
obtain information about blood flow. Perforator flaps are used in reconstructive
surgeries and the healthiest tissues are preferred. Such tissues can be identified
by studying the blood flow in the region of interest. Spectral information from
Doppler Ultrasound can be used to estimate the velocity of the blood flow. The
healthiest perforator is identified from the volumetric flow to have the largest
diameter, and it can be estimated by studying the energy of the Doppler shift
audio from the Continuous Wave Doppler Ultrasound.

# USAGE OF MATLAB CODE
1. Move all the MATLAB code, named below, in a single folder
(a) Wiener.m
It is a function file, which does noise reduction to enhance audio using
‘Wiener Filter’ algorithm.
(b) envelop_hilbert.m
It is a function file, which does ‘Voice Activity Detection (VAD)’ using Hilbert
transform algorithm.
(c) plot_doppler_samples.m
It is a script file, used to plot (time domain), play and does noise reduction of
Doppler audio samples.
(d) spectrogram_analysis.m
It is script file, used to do spectrogram analysis of Doppler audio samples.
(e) pitch_detection.m
It is a script file, used to estimate Doppler shift frequency in a Doppler audio
sample using Autocorrelation algorithm.
2. To obtain time domain plot, to play and to do the noise reduction of Doppler sample,
• Open plot_doppler_samples.m in MATLAB.
• To play audio, put the value of audio as 1 otherwise 0 in the line 5.
• To do the noise reduction, put the value of filter as 1 otherwise 0 in the line 6.
• Then RUN the file.
• File selection dialog box will open, then select the Doppler audio sample.
• OUTPUT:
i) Time domain plot.
17ii) Audio will play if play option selected.
iii) Noise reduced audio, if filter option selected and it will ask to save
the filtered audio in a folder specified by the user.
3. To do spectrogram analysis and to get velocity profile of Doppler audio sample,
• Open spectrogram_analysis.m in MATLAB.
• Enter the parameters of the equation (2.3) in the line 7, 8 and 9.
Default value of ‘Transmission frequency’ ft is 3.8 MHz and ‘Doppler angle’ theta
is 60 0 .
•
To get ‘Doppler shift frequency profile’ of the audio sample, put type as ‘freq’ and
To get ‘Blood Flow Velocity profile’ of the audio sample, put type as ‘Velocity’ in
the line 13.
•
To get ‘maximum’ and ‘average’ systolic peak velocity, put value of velocity as 1
otherwise 0 in the line 11.
• The RUN the file.
• File selection dialog box will open, then select the Doppler audio sample.
• OUTPUT:
i) Spectrogram plot, with frequency or velocity on y-axis as user
selected.
ii) Maximum and average systolic peak velocity will be displayed on
the command window.
4. To get Doppler shift frequency and thus blood flow velocity using autocorrelation
method,
• Open pitch_detection.m in MATLAB
• Enter the parameters of the equation (2.3) in the line 11, 12 and 13.
Default value of ‘Transmission frequency’ ft is 3.8 MHz and ‘Doppler angle’ theta
is 60 0 .
• The RUN the file.
• File selection dialog box will open, then select the Doppler audio sample.
• OUTPUT:
i) Blood flow velocity profile
ii) Maximum and average systolic peak velocity will be displayed on
the command window.
