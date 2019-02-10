# Mandarin_recognition_tf
A modified [DeepSpeech2](https://arxiv.org/abs/1512.02595) based Mandarin Recognition. Edit distance in valid data is 14.98% in [aishell](http://www.aishelltech.com/kysjcp) datasets.

## Train examples on valid sets
![Train Details](https://github.com/Novelfor/Mandarin_recognition_tf/blob/master/imgs/valid_results.png)

## More Details.
Train this model from audio to chinese character end-to-end. 

Use smaller (3x3) convolution kernel instead of 41x21 in paper get improved in valid set, and improve the speed for training model.

To improve the speed during decoding in dynamic GRU, we put the setences with similar length into a batch, and get 1.6x speed up for training model.

## A results:
![Predicts](https://github.com/Novelfor/Mandarin_recognition_tf/blob/master/imgs/examples.png)

## Pre-trained model download link.
[Dropbox](https://www.dropbox.com/s/g3p64r8eg1vrk20/CHINESE_CHARACTERS_19.zip?dl=0)

[Baidu](https://pan.baidu.com/s/1UgT7GjqChA7PSs8N-QC5BQ)
