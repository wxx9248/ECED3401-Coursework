# ECED3401-Coursework
ECED3401 (System Analysis) Coursework – 2020 Fall

## Copyright
Provided by [@Zackary-Lykos](https://github.com/Zackary-Lykos)

Author: Joshua Leon, PhD, Dalhousie University

## Preface
This is a project that I "stole" from Zack (lol). I am trying to complete the project from scrach, with pure C language, just for a programming exercise.

This project requires various skills that are related to signal processing, which I did not really dabble in before. To be honest, I feel this project is not simple **at all**, since I wanted to do signal processing from scrach, without any libraries (e.g. ffmpeg), and I didn't take any courses or teach my self on it, so it is a real challenge for me.

But hey, who don't like challenging and improving themselves? At lease I enjoy it!

## Requirements
Write software for editing wave files. The program must be able to read and write wave files and perform a number of editing functions on these sound files.

1. Add a track that is contained in another wave file. The original track can be sampled at a different rate, so files need to be normalized.
2. Create a mono file from a stereo file.
3. Create a loop track
    * i.e. Read a wave file and create a new wave file which repeats the original track `n` times.
4. Perform a low pass or high pass filter of the music. This involves:
    * taking an FFT of the original data and deleting components below a certain frequency (high-pass),
    *  or deleting components of above a certain frequency (low-pass).
5. Create a new file that plays the file at the speed `s` times faster or slower. `s` is a real number between `0.5` and `4`.
6. The system must be able to print out the recording details of a given file, i.e.,
    * Number of channels
    * Sampling rate
    * Samples per channel
    * Number of samples
    * The bits per sample
7. The interface can be a command line interface or can be data stored in a file. Each edit must be recorded in a history file. The history file stores the data about the edit.
    * Files involved
    * Parameters
    * Success or failure of the edits
    * Time of edit
8. The interface takes in the input filename or filenames, and parameters associated with the modifications.
