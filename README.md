# Myvoicerecognition

Speech Recognition wave2words

This package is a test sample and contains two functions and acts as a single program: 
a pronunciation/rhythm/stress words-phrases game (English). The package could be customized for
a speech-to-text system by accepting input from a microphone or an audio file or both. The 
package could be structured for any language of choice. 

In this package, we will test our wave2word speech recognition using AI, for English. However,
in the future releases, other languages will be added to make a language-independent speech
recognition. 

                                                  Concept

We may guess a word from unknown spoken languages just by listening to the sound of the Speech. 
To us, in an interaction between a human and a machine, the machine should recognise sounds before
making sense of any words (built from the combination of sounds) meaning. In other words, 
without pre-determining the language a speech recognition should pick up sounds and form words. 

Our speech processing system focuses on the process of understanding the acoustic features of 
sounds, then building words that are spoken by human beings. The speech signals are captured with 
the help of a microphone and then they are to be understood by the system.

The difficulty of speech recognition technology can be broadly characterised along some 
dimensions such as 1)size of a specific language vocabulary pool, 2)speaker dependency-sounds of
a particular word vary from a person to another, 3) the importance of channel quality; human speech
contains high bandwidth with full frequency range, while a telephone speech consists of low 
bandwidth with limited frequency range, 4)speaking mode that is whether the speech is in isolated
word mode, or connected word mode, or in a continuous speech mode. A continuous speech is 
harder to recognize, 5)speaking style; a loud-read speech, spontaneous and conversational, 6) type 
of the noise − signal to noise ratio may be in various ranges, depending on the acoustic environment
that observes less versus more background noise, 7) microphone quality and the distance between mouth 
and microphone. 

                                        Recording and Sampling

During recording with a microphone, the signals are stored in a digitised form. But to work upon it, 
the machine needs them in the discrete numeric form. Hence, our algorithm should sample the signals
at a particular frequency and convert the signal into the discrete numerical form. Choosing the high
frequency for sampling implies that when humans listen to the signal, they feel it as a continuous
audio signal.

                                     Transforming to Frequency Domain

Characterising an audio signal involves converting the time domain signal into the frequency domain, 
and understanding its frequency components that is an essential step because it gives a lot of information
about the signal. You can use a mathematical tool like Fourier Transform to perform this transformation. 
This transformation is the most critical step in building a speech recogniser because after converting the 
speech signal into the frequency domain, we must convert it into the usable form of the feature vector.
We can use different feature extraction techniques like MFCC, PLP, PLP-RASTA etc. for this purpose.

Myvoicerecognition is unique in its aim to provide a complete quantitative and analytical way to study the acoustic
features of a speech. Moreover, those features could be analysed further by employing Python's functionality
to provide more fascinating insights into speech patterns. 

This library is for Linguists, scientists, developers, speech and language therapy clinics and researchers. 
Please note that Myvoicerecognition Analysis is currently in the initial state though in active development. While 
the amount of functionality that is now present is not huge; more will be added over the next few months.


                                                   Installation

Myvoicerecognition can be installed like any other Python library, using (a recent version of) the Python package 
manager pip, on Linux, macOS, and Windows:

                                           pip install Myvoicerecognition  
or, to update your installed version to the latest release:

                                           pip install -u Myvoicerecognition 

NOTE: 
You need to get the following packages installed:

                    the Microsoft Visual C++ Redistributable for Visual Studio 2017 (x86 or x64, see your system)
                    PyAudio>= 0.2.11, pip install PyAudio (win),
                                      $ sudo apt-get install python-pyaudio python3-pyaudio (Debian-based Linux)
                                      $ brew install portaudio and then $ pip install pyaudio (MaC)
                    PyAudio-0.2.11-cp37-cp37m-win32.whl or win64.whl (if your system throws an error for PyAudio) 

you may get the third file from here https://github.com/Shahabks/Myvoicerecognition
save it in a directory and in cmd (command line)¬¬/directory/ pip install PyAudio-0.2.11-cp37-cp37m-winxx.whl.

The package uses the default system microphone. If your system has no default microphone, or you want to use 
a microphone other than the default, you will need to specify which one to use by supplying a device index. 

To check how the Myvoicerecognition functions behave, please check EXAMPLES.docx on 
https://github.com/Shahabks/Myvoicerecognition

                                                  Development

Myvoicerecognition was developed by MYOLUTIONS Lab in Japan. It is part of New Generation of Voice
Recognition and Acoustic & Language modeling Project in MYSOLUTIONS Lab. That is planned to enrich 
the functionality of Myvoicerecognition by adding more advanced functions.
