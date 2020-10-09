# py3pYIN
Python3 version of pYIN (pitch and note tracking for monophonic audio), adapted from https://github.com/ronggong/pypYIN.


## pYIN project page
[https://code.soundsoftware.ac.uk/projects/pyin](https://code.soundsoftware.ac.uk/projects/pyin)


## Dependencies
Numpy  
Scipy  
Essentia  

## Usage

### Initialise:  
Here are the parameters which need to be initialised before executing the main program:  

inputSampleRate:      sampling rate
stepSize:             hopSize  
blockSize:            frameSize  
lowAmp(0,1):          RMS of audio frame under lowAmp will be considered non voiced  
onsetSensitivity:     high value means note is easily be separated into two notes if low amplitude is presented.  
pruneThresh(second):  discards notes shorter than this threshold

### Output:
Transcribed notes in Hz  
Smoothed pitch track  
Pitch tracks of transcribed notes in MIDI note number  

### Other issues:
See demo.py

## References 

 > M. Mauch and S. Dixon,  
 > “pYIN: A Fundamental Frequency Estimator Using Probabilistic Threshold Distributions”,  
 > in Proceedings of the IEEE International Conference on Acoustics,  
 > Speech, and Signal Processing (ICASSP 2014), 2014.  
 
 > M. Mauch, C. Cannam, R. Bittner, G. Fazekas, J. Salamon, J. Dai, J. Bello and S. Dixon,  
 > “Computer-aided Melody Note Transcription Using the Tony Software: Accuracy and Efficiency”,  
 > in Proceedings of the First International Conference on Technologies for  
 > Music Notation and Representation, 2015.  

