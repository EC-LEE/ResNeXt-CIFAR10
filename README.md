# ResNeXt-CIFAR10
pytorch code for resnext on CIFAR10

This implementation is for studying the ResNeXt paper, "Aggregated Residual Transformations for Deep Neural Networks, \
Saining Xie, Ross Girshick, Piotr Dollár, Zhuowen Tu, Kaiming He (2016)".


# Details
I tried to make it exactly the same as described in the paper(see Sec 5.3 of the Xie's paper), but except these things.
1. per-pixcel mean substraction is not used, but instead I nomalized with (0.5,0.5).

# Results
||ResNet_l-29|ResNeXt-29|
|------|---|---|
|Test|--% (err --%)|--% (err --%)|
|Paper|--% (err --%)|--% (err --%)|
