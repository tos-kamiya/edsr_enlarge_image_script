## EDSR enlarge-image script

A helper script to enlarge image files with the [EDSR](https://github.com/Saafke/EDSR_Tensorflow) model.

## Requirements

* Tensorflow
* OpenCV + contrib
* EDSR model
* docopt

```sh
pip3 install tensorflow-cpu  # or tensorflow-gpu, depending on your environmnet
```

```sh
pip3 install opencv-python
pip3 install opencv-contrib-python
pip3 install docopt
```

Download model files (`EDSR_x2.pb`, `EDSR_x3.pb`, `EDSR_x4.pb`) from:

https://github.com/Saafke/EDSR_Tensorflow

and copy them into the directory of a script `image_x`.

## Usage

```sh
image_x 2 image.jpg  # outputs `image-x2.jpg`
```

## References

EDSR in Tensorflow https://github.com/Saafke/EDSR_Tensorflow

Deep Learning based Super Resolution with OpenCV https://towardsdatascience.com/deep-learning-based-super-resolution-with-opencv-4fd736678066

ImportError: cannot import name 'dnn_superres' for python example of super resolution with opencv https://stackoverflow.com/questions/61159469/importerror-cannot-import-name-dnn-superres-for-python-example-of-super-resol
