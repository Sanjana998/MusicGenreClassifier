# MusicGenreClassifier

Music plays a very important role in people’s lives. Music 
brings like-minded people together and is the glue that holds 
communities together. One main feature that separates one kind of 
music from another is the genre of the music.
The aim of this project is to build a machine learning model 
which classifies music into its respective genre.

Applied KNN,Random forest,SVC algorithms
The data set is taken from GTZAN


Dataset Description:
	
The dataset consists of 1000 audio tracks each 30 seconds long. It contains 10 genres, each represented by 100 tracks. The tracks are all 22050 Hz monophonic 16-bit audio files in .wav format.
The dataset can be download from a data repository called www.kaggle.com
The dataset consists of 10 genres i.e

Data Set Features

These features are extracted from the audio tracks :
Time Domain Features :
•	Zero Crossing Rate (ZCR): This point is where the signal changes sign from positive to negative. The entire 30 second signal is divided into smaller frames, and the number of zero-crossings present in each frame are determined. The average and standard deviation of the ZCR across all frames are chosen as representative features.

•	Root Mean Square Energy (RMSE): The energy signal in a signal is calculated as RMSE is calculated frame by frame and then the average and standard deviation across all frames is taken

•	Tempo: Tempo refers to the how fast or slow a piece of music is. Tempo is expressed in terms of Beats Per Minute (BPM). We take the aggregate mean of the Tempo as it varies from time to time.
	 Frequency Domain Features:

•	Mel-Frequency Cepstral Coefficients (MFCC): Introduced in the early 1990s by Davis and Mermelstein, MFCCs have been very useful features for tasks such as speech recognition.

•	 Chroma Features: This is a vector which corresponds to the total energy of the signal in each of the 12 pitch classes. (C, C#, D, D#, E ,F, F#, G, G#, A, A#, B). Then the aggregate of the chroma vectors is taken to get the mean and standard deviation. 

•	Spectral Centroid: This corresponds to the frequency around which most of the energy is centered. It is a magnitude weighted frequency calculated as: where S(k) is the spectral magnitude of frequency bin k and f(k) is the frequency corresponding to bin k.

•	Spectral Contrast: Each frame is divided into a prespecified number of frequency bands. And, within each frequency band, the spectral contrast is calculated as the difference between the maximum and minimum magnitudes.

•	Spectral Roll-off: This feature corresponds to the value of frequency below which 85% of the total energy in the spectrum lies.

•	And other features like audio file name, audio track length(duration), label ,spectral bandwidth ,harmony and  preceptor.
The mean and standard deviation of the values taken across frames is considered as the representative final feature that is fed to the model.

