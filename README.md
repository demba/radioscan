## Installing `radiopy` package from pip to record streaming audio

First trying installing the usual way with pip:

`pip install radiopy`

`pip` failed to find the package this way on my Ubuntu box. The following worked

`pip install git+http://git.code.sf.net/p/radiopy/code`

## Testing radio py installation

### List preset/available radio stations

The package comes with a list of pre-configured radio stations. List them as follows,

`radio.py -l`

### Start listening to *Loca FM* and stop after 1 minute
`radio.py -s 1 Loca FM`

### Start listening to *Loca FM* in 1 minute

`radio.py -w 1 Loca FM`

This command fires up *Loca FM* after 1 minute time has passed.

### Listen to and record from *Loca FM* for 1 minute

`radio.py -r loca2 -s 1 Loca FM`

### For help

`radio.py -h`

## Installing `SpeechRecognition` package from PyPi

### Install package

`pip install SpeechRecognition`

### Testing installation

To test this package after installation, you must install [pyaudio](https://people.csail.mit.edu/hubert/pyaudio/), which requires v19 (at the time of this writing) of the [portaudio]() library.

### Download and compile `portaudio`

Download [portaudio](http://www.portaudio.com/download.html) and follow the [instructions](http://portaudio.com/docs/v19-doxydocs/tutorial_start.html) to build the source/install for your OS.

Upone successful installation, a "Successfully installed" installed message, or something to that effect, should be output to your terminal.

### Install `pyaudio` using pip

`pip install http://people.csail.mit.edu/hubert/pyaudio/packages/pyaudio-0.2.8.tar.gz`

### Test `SpeechRecognition` from the command line

**N.B.: The testing script looks like it is web-based. Make sure you have internet connectivity!**


 `python -m speech_recognition`

 Say something sweet to your mic! It will output to the screen what it recognizes!
