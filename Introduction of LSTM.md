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


#### LSTM-PTB
* PTB_Single        55(服务器）
* PTB_Baseline      无（服务器）                  60(天河)
* PTB_Aji_Momentum_Corr   67.84(服务器)          67.59(天河)
* PTB_Var_Momentum_Corr   66.25(服务器)          68.01(天河)
* PTB_Baseline_Adj  无（服务器）                  68.43/70(天河)
* PTB_Aji           无 (服务器）                  无收敛(天河)


#### ResNet18-Tiny_ImageNet_200
* ResNet18_Single    0.3904， 0.6365(服务器)          (天河)
* ResNet18_Baseline    无(服务器)     (天河)
* ResNet18_Aji           (服务器)     (天河)
* ResNet18_Var_Momentum  (服务器)     (天河)
* ResNet18_Var_Momentum_Corr  (服务器)     (天河)




