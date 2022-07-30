# Watermark detection

A model trained for watermark detection using Tensorflow.

## Run

The code and description can be found in [watermark-detector.ipynb](watermark-detector.ipynb).

The dataset is expected to be in the same directory as the notebook. But you can change `base_dir` variable in the notebook to point to the arbitrary dataset parent directory. 

Another version of code using pre-trained ResNet50 on "imagenet" dataset as the base model
for transfer learning is also available in [watermark-detector-transfer-learning.ipynb](watermark-detector-transfer-learning.ipynb).

## Dataset

The dataset contains images from Digikala, an Iranian online shop, some including various kinds of watermarks. The data is labeled with `positive` or `negative,` indicating whether the image has or has not watermark respectevly.

The dataset structure is as follows:

```
dataset
    / train
        / positive
        / negative
    / test
```

Data can be accessed 
from [here](https://drive.google.com/file/d/1JWpW6JTdV__L-j18QU3wgGrcIdguHl8l/view?usp=sharing).

There are 8582 samples for training and 1103 unlabeled samples for testing.

You can submit your testing prediction result in [Quera](https://quera.org/problemset/138169/) (the problem statement is in Persian) and get the accuracy of the model on the test data. 
