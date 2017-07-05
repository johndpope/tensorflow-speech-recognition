# Tensorflow Speech Recognition
Speech recognition using google's [tensorflow](https://github.com/tensorflow/tensorflow/) deep learning framework, [sequence-to-sequence](https://www.tensorflow.org/versions/master/tutorials/seq2seq/index.html) neural networks.

Replaces [caffe-speech-recognition](https://github.com/pannous/caffe-speech-recognition), see there for some background.

## Ultimate goal
Create a decent standalone speech recognition for Linux etc.
Some people say we have the models but not enough training data.
We disagree: There is plenty of training data (100GB [here](http://www.openslr.org/12) and 21GB [here on openslr.org](http://www.openslr.org/7/) , synthetic Text to Speech snippets, Movies with transcripts, Gutenberg, YouTube with captions etc etc) we just need a simple yet powerful model. It's only a question of time...

![Sample spectrogram, That's what she said, too laid?](images/0_Karen_160.png)

Sample spectrogram, Karen uttering 'zero' with 160 words per minute.

## Getting started

Toy examples:
`./number_classifier_tflearn.py`
`./speaker_classifier_tflearn.py`

Some less trivial architectures:
`./densenet_layer.py`

Later:
`./train.sh`
`./record.py`

![Sample spectrogram or record.py](images/spectrogram.demo.png)

## Partners + collaborators wanted
We are in the process of tackling this project in seriousness. If you want to join the party just drop us an email at [info@pannous.com](mailto:info@pannous.com?subject=speech_recognition).
<!-- ╮⚆ᴥ⚆╭ -->

Update: Nervana [demonstrated](https://www.youtube.com/watch?v=NaqZkV_fBIM) that it is possible for 'independents' to build speech recognizers that are state of the art. 
Update: **Mozilla** is working on [DeepSpeech
](https://github.com/mozilla/DeepSpeech) and just achieved [0% error rate](http://doyouunderstand.me) ... on the training set;) Free Speech is in good hands.
**Samsung SDS-RN** - port of Baidu deepspeech to use  [mxnet
](https://github.com/samsungsds-rnd/deepspeech.mxnet).


<!-- ᖗ*﹏*ᖘ -->

### Fun tasks for newcomers
* Watch video : https://www.youtube.com/watch?v=u9FPqkuoEJ8
* Understand and correct the corresponding code: [lstm-tflearn.py](/lstm-tflearn.py) 
* Data Augmentation :  create on-the-fly modulation of the data: increase the speech frequency, add background noise, alter the pitch etc,...
<!-- ᕮ◔‿◔ᕭ -->

### Extensions 
**Extensions** to current tensorflow which are probably needed:
* [WarpCTC on the GPU](https://github.com/baidu-research/warp-ctc/tree/master/tensorflow_binding) see [issue](https://github.com/tensorflow/tensorflow/issues/2146)
* Incremental collaborative snapshots ('[P2P learning](https://github.com/pannous/tensorpeers)') !
* Modular graphs/models + persistance
<!-- ⤜(⨱ᴥ⨱)⤏ -->

Even though this project is far from finished we hope it gives you some starting points.

Looking for a tensorflow collaboration / consultant / deep learning contractor? Reach out to [info@pannous.com](mailto:info@pannous.com?subject=contractor)
<!--
 Notes
STT https://github.com/sotelo/parrot/blob/master/model.py t
 parrot

-->
