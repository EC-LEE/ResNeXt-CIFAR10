# ResNeXt-CIFAR10
pytorch code for resnext on CIFAR10

This implementation is for studying the ResNeXt paper, "Aggregated Residual Transformations for Deep Neural Networks, \
Saining Xie, Ross Girshick, Piotr Dollár, Zhuowen Tu, Kaiming He (2016)".


# Details
I tried to make it the same as described in the paper (see Sec 5.3 of the Xie's paper), but except for these things.
1. per-pixcel mean substraction is not used, but instead I nomalized with (0.5,0.5).
2. Though the learning rate started from  '0.1' in the paper, I used '0.01' because training model exploded when the lr started from '0.1'.

# Results
|aaaaaaaaaaa|ResNeXt-29(increase cardinality)|
|------|---|---|
|ResNet-29(increase width)|--% (err --%)|--% (err --%)|
|ResNeXt-29(increase cardinality)|--% (err --%)|--% (err --%)|

![제목 없음1](https://user-images.githubusercontent.com/20814465/124403509-d33d8780-dd71-11eb-82be-8e67cbe28428.png)


* results of the paper<br/>
![제목 없음](https://user-images.githubusercontent.com/20814465/124236121-0ead3b80-db51-11eb-9b2f-cbb8b63363ec.png)
