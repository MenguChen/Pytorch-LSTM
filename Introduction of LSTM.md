### LSTM相关说明

#### LSTM模型说明
https://zhuanlan.zhihu.com/p/32085405

#### Pytorch在LSTM模型下训练PTB数据
https://github.com/pytorch/examples

#### GRU-AN4
* AN4_Single    20
* AN4_Baseline  未测试
* AN4_Aji       41
* AN4_Var       46


python LSTM_Baseline.py --init-method='file:///HOME/sysu_wgwu_5/share_file_chenmq' --dist-rank 0
四个节点以上，需要添加：net = torch.nn.parallel.DistributedDataParallel(net) 否则，准确率无法保障

#### LSTM-PTB
* PTB_Single        55(服务器）
* PTB_Baseline      无（服务器）                  60(天河)
* PTB_Aji_Momentum_Corr   67.84(服务器)          67.59(天河)
* PTB_Var_Momentum_Corr   66.25(服务器)          68.01(天河)
* PTB_Baseline_Adj  无（服务器）                  68.43/70(天河)
* PTB_Aji           无 (服务器）                  85(天河)


#### ResNet50-Tiny_ImageNet_200
* ResNet50_Single    0.4280 0.6705(服务器)          (天河)
* ResNet50_Baseline      (服务器)     (天河)
* ResNet50_Aji           (服务器)     (天河)
* ResNet50_Var_Momentum  (服务器)     (天河)
* ResNet50_Var_Momentum_Corr  (服务器)     (天河)


#### ResNet18-Tiny_ImageNet_200
* ResNet18_Single    0.4216 0.6751(服务器)          (天河)
* ResNet18_Baseline      (服务器)     0.3798 0.6335(天河2)    0.3683 0.6210（天河4带Parallel)  
* ResNet18_Aji           (服务器)     0.3916 0.6443(天河2)    0.4009 0.6557 (天河4带Parallel)
* ResNet18_Var_Momentum  (服务器)     0.3828 0.6377(天河2)    0.4093 0.6556 (天河4带Parallel)
* ResNet18_Var_Momentum_Corr  (服务器)    03947 0.6481 (天河2)


#### VGG-Cifar10
* VGG_Single    0.9119(服务器)          (天河)
* VGG_Baseline    无(服务器)          0.8857(天河)
* VGG_Aji           (服务器)          0.8953(天河)
* VGG_Var_Momentum  (服务器)          0.8920(天河)
* VGG_Var_Momentum_Corr  (服务器)     0.8978(天河)

#### AlexNet-Cifar10
* AlexNet_Single    0.7474(服务器)          (天河)
* AlexNet_Baseline    无(服务器)     0.7292(天河)
* AlexNet_Aji           (服务器)     0.7303(天河)
* AlexNet_Var_Momentum  (服务器)     0.7094(天河)
* AlexNet_Var_Momentum_Corr  (服务器)     0.7338(天河)


