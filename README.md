# Digital-Signal-Processing
💭 NTUA ECE DSP and Course Source Codes in Python

### Lab1

The whole assesemnt consists of three parts:

The first part had to do with tracking telephone touch-tones. Each digit can be described as the sum of two sines so we write them this way and we record a sequence in a .wav file. We then plot the recorded signal using hamming and rectangular windows. After that, we calculate the coordinates of the peak of each digit by calculating the frequency from crossings. Lastly, with two different signals as input, we have to decode the digits in them and print them.

The second part has to do with Short Time Fourier Transform (STFT) and Wavelets Transform (Discrete Time CWT). We first plot the stft of a signal and then its absolute CWT in the fields of both time and frequency and compare the analysis quality of each transform. By adding some white noise and dirac deltas we perform the same tasks and we see that DTCWT is inferior to the STFT due to the noise.

The third part has to do with short term energy and crossing rate of voice and music signals. Using a hamming window we calculate the above from the speech_utterance.wav file and compare them with the respective results from the music.wav file. We came to the conclusion that wider window means less precise short term energy and that gaussian noise reduces the crossing rate of the silent spots. This is why we cannot distinguish loud(periodical and wide) from silent noises(aperiodical).

### Lab2

The whole assesment consists of four parts:

The first part has to do with calculating short time energy and stft of movement and heart rate signals. By reading a file, we plot its components (acc, gyr, hrm) in all axis. Then we calculate and plot their short time energies, as well as their STFTs. Lastly, we define the characteristics of a signal (mean, min, max, standard deviation) and, by comparing sleep_03.npz and step_03.npz, we see that what distinguishes a sleeping from an awake person is the
standard deviation,min,max.If a person's heart rate has high maximums and low minimums, as well as high standard deviation, then the person is awake. Else, he is asleep.

The second part has to do with calculating Teager-Kaiser energy in multiple frequency layers by using Gabor filterbank.

The third part was optional.

The fourth part has to do with reducing the noise of movement signals by using Butterworth and Wiener filter.
