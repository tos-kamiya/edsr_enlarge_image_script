## EDSR画像拡大スクリプト

[EDSR](https://github.com/Saafke/EDSR_Tensorflow)のモデルを利用して画像ファイルを拡大するヘルパースクリプト。

## 必要なもの

* Tensorflow
* OpenCV + contrib
* EDSR model
* docopt

```sh
pip3 install tensorflow-cpupip3 install opencv-python
pip3 install opencv-contrib-python
pip3 install docopt
```

モデルファイル(`EDSR_x2.pb`, `EDSR_x3.pb`, `EDSR_x4.pb`)を次から入手して、

https://github.com/Saafke/EDSR_Tensorflow

`image_x`スクリプトを置いているディレクトリにコピーしてください。

**注意** スクリプトをcuDNN+Cuda+Nvidia GPUの環境で動かしたいときは、OpenCVをNvidia GPU向けにセットアップする必要があります。OpenCVレポジトリの[関連するイシュー](https://github.com/opencv/opencv/issues/15858)を参考にしてください。

## 利用方法

```sh
image_x 2 image.jpg  # `image-x2.jpg`を出力する
```

## 参考

EDSR in Tensorflow https://github.com/Saafke/EDSR_Tensorflow

Deep Learning based Super Resolution with OpenCV https://towardsdatascience.com/deep-learning-based-super-resolution-with-opencv-4fd736678066

ImportError: cannot import name 'dnn_superres' for python example of super resolution with opencv https://stackoverflow.com/questions/61159469/importerror-cannot-import-name-dnn-superres-for-python-example-of-super-resol
