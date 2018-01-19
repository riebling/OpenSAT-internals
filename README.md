# Diarization Using Noisemes (formerly known as OpenSAT) - 
The diarization stuff inside the (Diarization) VM
which can now be found at http://github.com/srvk/DiarizationVM

New usage supports multiple files

  * Start with a folder full of .wav files to be processed
  * Path to the root folder (here! "OpenSat")
  * give the command ./runDiarNoisemes.sh <folder holding .wav files>

The system will grind first creating features for all the .wav files it found, then will place those features in a subfolder `feature`. Then it will load a model, and process all the features generated, producing output in a subfolder `hyp` as two files (for now): `confidence.mat` and `confidence.pkl.gz` - a confidence matrix in Matlab v5 mat-file format, and a Python compressed data 'pickle' file

