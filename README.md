# DogsVSCats_learn_1
Run the full PyTorch code for the first time. Thanks for 你的雷哥 (https://www.cnblogs.com/henuliulei/p/12081560.html)


数据集下载地址https://www.kaggle.com/c/dogs-vs-cats-redux-kernels-edition/data

图片经过data_transforms处理完大小为224*224*3
卷积层 conv1设置：in_channels=3,out_channels=6,kernel_size=5*5,stride=1,padding=0
            得到输出: 220*220*6
最大池化层 Maxpool设置：kernel_size=2*2,stride=2
              得到输出: 110*110*6
卷积层 conv2设置：in_channels=6, out_channels=16, kernel_size=5*5, stride=1, padding=0
        得到输出：106*106*16
最大池化层 Maxpool设置：kernel_size=2*2,stride=2
         得到输出: 53*53*16
全连接层：53*53*16--->1024
全连接层：1024--->512
全连接层：512--->2

