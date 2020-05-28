# LIGO_Data-Challenge_2020
GW Open Data Workshop #3
Challenge activity for the Open Data Workshop 2020: https://www.gw-openscience.org/s/workshop3/

#Data files may be downloaded using these links:


[challenge1.gwf](https://www.gw-openscience.org/s/workshop3/challenge/challenge1.gwf)

[challenge2.gwf](https://www.gw-openscience.org/s/workshop3/challenge/challenge2.gwf)

[challenge3.gwf](https://www.gw-openscience.org/s/workshop3/challenge/challenge3.gwf)

##Challenge 1 (1 point) -- Novice
Identify a loud binary black hole signal in white, Gaussian noise.

Use the data file "challenge1.gwf". The channel name is "H1:CHALLENGE1".
The data are white, Gaussian noise containing a simulated BBH signal.
Load the data into memory. What are the sampling rate and duration of the data?

Plot the data in the time-domain.

Plot a spectrogram (or q-transform) of the data, and try to identify the signal.

What is the time of the merger?

##Challenge 2 (2 points) -- Rookie
Signal in colored, Gaussian noise.

Use the data file "challenge2.gwf", with channel name "H1:CHALLENGE2"
The data contain a BBH signal with m1=m2=30 solar masses, spin = 0.
What is the approximative time of the merger? (Hint: a plot of the q-transform could help)

Generate a time-domain template waveform using approximate "SEOBNRv4_opt". with the same parameters as above. Plot this waveform.

Calculate a PSD of the data, and plot this on a log-log scale. Use axes ranging from 20 Hz up to the Nyquist frequency.

Use the template waveform and PSD to calculate the SNR time series. Plot the SNR time-series.

What is the matched filter SNR of the signal?

##Challenge 3 (4 points) -- Intermediate
Use the data file "challenge3.gwf" with channel "H1:CHALLENGE3"
These are real LIGO data from O2, though we've adjusted the time labels and added some simulated signals.
The data contain a loud simulated signal with m1 = m2 = 10 solar masses.
What is the merger time of this signal?

What is the matched-filter SNR of this signal?

Challenge 4 (8 points) -- Advanced
Use the data file "challenge3.gwf" with channels "H1:CHALLENGE3" and "L1:CHALLENGE3".
These are real LIGO data from O2, though we've adjusted the time labels and added some simulated signals.
Any simulated signals have been added to both the H1 and L1 data
All simulated signals have 0 spin and m1=m2, with m1 somewhere in the range 10-50 solar masses
Identify as many signals as you can. Watch out! These are real data, and so glitches may be present. Any correct detection is +1 point but any false alarms will count -1 point against your score. For each signal you find, list:
The merger time
The SNR
Your estimate of the component masses
Identify as many glitches as you can. Make a spectrogram of each one.

For each simulated BBH you found, use bilby to compute a posterior distribution for the mass. You can fix the spin and mass ratio to make this run faster.
