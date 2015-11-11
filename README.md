# MITIE-Writer
(pronounced "Mighty Writer") A PyQt text editor that highlights named entities as you type.  It also saves the entity data to your harddrive for easy querying and management of your documents later on.

![Early Function Example](https://github.com/nickstanisha/MITIE-Writer/blob/master/screenshots/mitie_1.PNG)

## Prerequisites
* Python 2.7
* [MITIE](https://github.com/mit-nlp/MITIE) state-of-the-art information extraction tool
* PyQt4
* nltk

Launch the text editor with `python app.py`

### Language Menu
![Loading a language Model](https://github.com/nickstanisha/MITIE-Writer/blob/master/screenshots/loadMITIE.PNG)

The Language menu enables several functions:
* **Load language model** - Allows you to navigate to a MITIE language model to use for named entity recognititon.  You can use the [English or Spanish models provided by MITIE](https://github.com/mit-nlp/MITIE#initial-setup) or you can [train your own](https://github.com/mit-nlp/MITIE/blob/master/examples/python/train_ner.py).
* **Refresh Entity Tags** - Relabels entities in your document.  By default, MITIE-Writer reevaluates the entities whenever there is a textChanged event and the resulting document is a set of complete sentences (fragments are not sent for labeling)
* **Change Tag Colors** - Change the highlighting colors for different tags.  By default, 'Person' is red, 'Location' is blue, 'Organization' is green, and 'Miscellaneous' is purple.
* **Toggle Highlighting** - Turn entity highlighting on/off.  Note that this only changes the appearance of your text editor, your entities are still being recorded.

### Saving entities to disk
Entities are now automatically saved to their own [.entities file](https://github.com/nickstanisha/MITIE-Writer/wiki/.entities-file) whenever the document is saved.

### Upcoming Features
* User-added entity tags


#### Note
This was originallly a fork of [Peter Goldsborough's Writer-Tutorial project](https://github.com/goldsborough/Writer-Tutorial).  See his [original README.md](https://github.com/goldsborough/Writer-Tutorial/blob/master/README.md) for additional information.
