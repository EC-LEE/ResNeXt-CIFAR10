# ResNeXt-CIFAR10
pytorch code for resnext on CIFAR10

This implementation follows the ResNeXt paper, "Aggregated Residual Transformations for Deep Neural Networks, \
Saining Xie, Ross Girshick, Piotr Dollár, Zhuowen Tu, Kaiming He (2016)".


# Details
I tried to make it the same as described in the paper (see Sec 5.3 of the Xie's paper), but except for these things.
1. I uesd learnig rate 0.05 instead of 0.1.

# Results
||64d|92d/2x64d|128d/3x64d|160d/4x64d|
|------|---|---|---|---|
|ResNet-29(increase width)|95.58% (err 4.42%)|95.87% (err 4.13%)|--% (err --%)|--% (err --%)|
|ResNeXt-29(increase cardinality)||95.98% (err 4.02%)|--% (err --%)|96.2% (err 3.8%)|


![제목 없음](https://user-images.githubusercontent.com/20814465/124525269-9e950300-de39-11eb-9fd0-953b5cb84ee5.png)

* results show 1x64d < 96d < 2x64d
* 96d and 2x64d models have similar complexity.<br/>
* all scores are slightly lower than paper, and I'm fixing it.

-----------------------------------------------
![제목 없음](https://user-images.githubusercontent.com/20814465/124236121-0ead3b80-db51-11eb-9b2f-cbb8b63363ec.png)
* results of the paper<br/>
