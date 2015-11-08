# MITIE-Writer
(pronounced "Mighty Writer") A PyQt text editor that keeps track of named entities as you type.

![Early Function Example](https://github.com/nickstanisha/MITIE-Writer/blob/master/screenshots/mitie_1.PNG)

## Prerequisites
* Python 2.7
* [MITIE](https://github.com/mit-nlp/MITIE) state-of-the-art information extraction tool
* PyQt4
* nltk

Launch the text editor with `python app.py`

## Loading a Language Model
![Loading a language Model](https://github.com/nickstanisha/MITIE-Writer/blob/master/screenshots/loadMITIE.PNG)

Using the "Language" button on the menu bar to navigate to a MITIE language model to use for named entity recognititon.  You can use the [English or Spanish models provided by MITIE](https://github.com/mit-nlp/MITIE#initial-setup) or you can [train your own](https://github.com/mit-nlp/MITIE/blob/master/examples/python/train_ner.py).

## Upcoming Features
* Saving document entities to disk
* In-text highlighting for entities
* Increased memory efficiency for calls to MITIE


#### Note
This was originallly a fork of [Peter Goldsborough's Writer-Tutorial project](https://github.com/goldsborough/Writer-Tutorial).  See his [original README.md](https://github.com/goldsborough/Writer-Tutorial/blob/master/README.md) for additional information.
