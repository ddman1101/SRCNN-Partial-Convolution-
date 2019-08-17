# SRCNN-Partial-Convolution
Using Partial Convolution with Zero-Padding in SRCNN 

## 必備
 * Tensorflow
 * Scipy version > 0.18 ('mode' option from scipy.misc.imread function)
 * h5py
 * matplotlib

## 使用
For training, `python main.py --is_train True`
<br>
For testing, `python main.py --is_train False`

## 結果
經過訓練15000次，達到效果如下：<br>
![Ground truth](https://github.com/ddman1101/SRCNN-Partial-Convolution-/blob/master/padding_label.png)<br>
Bicubic Interpolated image:<br>
![Bicubic Interpolation (2倍)](https://github.com/ddman1101/SRCNN-Partial-Convolution-/blob/master/bi2_baby.png)<br>
訓練0次:<br>
![SRCNN(Partial Convolution)-Training 0 epoch](https://github.com/ddman1101/SRCNN-Partial-Convolution-/blob/master/set5-0-0.png)
訓練15000次:<br>
![SRCNN(Partial Convolution)-Training 15000 epoch](https://github.com/ddman1101/SRCNN-Partial-Convolution-/blob/master/set5-15000-0.png)

## 訓練時間以及使用電腦設備
訓練15000次之時間：2小時15分鐘9秒
CPU : i7-8750H 2.2GHz RAM : 32GB，GPU : RTX2080。

## 參考
* [tegg89/SRCNN-Tensorflow](https://github.com/tegg89/SRCNN-Tensorflow) 
<br>
