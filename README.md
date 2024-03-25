# LibContinual
Make continual learning easy.

## Supported Methods
+ [BiC (CVPR 2019)](https://github.com/RL-VIG/LibContinual/blob/master/reproduce/bic/README.md)
+ [EWC (PNAS 2017)](https://github.com/RL-VIG/LibContinual/blob/master/reproduce/ewc/README.md)
+ [iCaRL (CVPR2017)](https://github.com/RL-VIG/LibContinual/blob/master/reproduce/icarl/README.md)
+ [LUCIR (CVPR 2019)](https://github.com/RL-VIG/LibContinual/blob/master/reproduce/lucir/README.md)
+ [LwF (ECCV 2016)](https://github.com/RL-VIG/LibContinual/blob/master/reproduce/lwf/README.md)
+ [WA (CVPR 2020)](https://github.com/RL-VIG/LibContinual/blob/master/reproduce/wa/README.md)
+ [OCM (PMLR 2022)](https://github.com/RL-VIG/LibContinual/blob/master/reproduce/ocm/README.md)
+ [DER (CVPR 2021)](https://github.com/RL-VIG/LibContinual/blob/master/reproduce/der/README.md)


## Quick Installation
(待文档部分完成)  <br>
请参考文档中[`安装`](https://github.com/RL-VIG/LibContinual/blob/master/docs/tutorials/install.md)部分。 <br>
完整文档：[`./docs`](https://github.com/RL-VIG/LibContinual/tree/master/docs)

## Datasets
[`CIFAR-100`](https://drive.google.com/drive/folders/1EL46LQ3ww-F1NVTwFDPIg-nO198cUqWm?usp=sharing), `miniImageNet(todo)`  <br>

将对应数据集的压缩包解压至指定路径:
```
unzip cifar100.zip -d /path/to/your/dataset
```
修改.yaml文件的data_root参数：
```
data_root: /path/to/your/dataset
```
如何添加自定义数据集请参考文档:[`添加自定义数据集`](https://github.com/RL-VIG/LibContinual/blob/master/docs/tutorials/data_module.md)

## Get Start

当您已经完成`Quick Installation`和`Datasets`后，我们以`LUCIR`方法为例展示如何使用`LibContinual`。
- **Step1: 修改`run_trainer.py`中`Config`参数为`./config/lucir.yaml`**
- **Step2：配置`./config/lucir.yaml`文件中的参数，各参数含义请参考[配置文件](https://github.com/RL-VIG/LibContinual/blob/master/docs/tutorials/config_file.md)**
- **Step3: 运行代码`python run_trainer.py`**
- **Step4：日志保存在配置文件中`save_path`路径下**



## Acknowledgement
LibContinual is an open source project designed to help continual learning researchers quickly understand the classic methods and code structures. We welcome other contributors to use this framework to implement their own or other impressive methods and add them to LibContinual. This library can only be used for academic research. We welcome any feedback during using LibContinual and will try our best to continually improve the library.

## License
This project is licensed under the MIT License. See LICENSE for more details.