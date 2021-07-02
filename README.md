# ResNeXt-CIFAR10
pytorch code for resnext on CIFAR10

This implementation is for studying the ResNeXt paper, "Aggregated Residual Transformations for Deep Neural Networks, \
Saining Xie, Ross Girshick, Piotr Dollár, Zhuowen Tu, Kaiming He (2016)".


# Details
I tried to make it the same as described in the paper (see Sec 5.3 of the Xie's paper), but except for these things.
1. per-pixcel mean substraction is not used, but instead I nomalized with (0.5,0.5).

# Results
||ResNet-29(increase width)|ResNeXt-29(increase cardinality)|
|------|---|---|
|Test|--% (err --%)|--% (err --%)|
|Paper|--% (err --%)|--% (err --%)|

⋅⋅* results of the paper<br/>
![제목 없음](https://user-images.githubusercontent.com/20814465/124236121-0ead3b80-db51-11eb-9b2f-cbb8b63363ec.png)
