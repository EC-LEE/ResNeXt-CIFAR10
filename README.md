# ResNeXt-CIFAR10
pytorch code for resnext on CIFAR10

This implementation follows the ResNeXt paper, "Aggregated Residual Transformations for Deep Neural Networks, \
Saining Xie, Ross Girshick, Piotr Dollár, Zhuowen Tu, Kaiming He (2016)".


# Details
I tried to make it the same as described in the paper (see Sec 5.3 of the Xie's paper), but except for these things.
1. per-pixcel mean substraction is not used, but instead I nomalized with (0.5,0.5).
2. Though the learning rate started from  '0.1' in the paper, I used '0.01'. Training model exploded when the lr started from '0.1'.

# Results
||64d|92d/2x64d|128d/3x64d|160d/4x64d|
|------|---|---|---|---|
|ResNet-29(increase width)|94.96% (err 5.04%)|--% (err --%)|95.18% (err 4.82%)|--% (err --%)|
|ResNeXt-29(increase cardinality)||--% (err --%)|95.57% (err 4.43%)|--% (err --%)|


![제목 없음1](https://user-images.githubusercontent.com/20814465/124403666-7f7f6e00-dd72-11eb-9dad-3023b5be890b.png)
* results show 1x64d < 128d < 3x64d
* 128d and 3x64d models have similar complexity.<br/>
* all scores are slightly lower than paper, and I'm fixing it.

-----------------------------------------------
![제목 없음](https://user-images.githubusercontent.com/20814465/124236121-0ead3b80-db51-11eb-9b2f-cbb8b63363ec.png)
* results of the paper<br/>
