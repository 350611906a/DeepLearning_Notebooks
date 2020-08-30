# 深度学习的注意事项记录 

## 配置库方法

1、在pycharm中加载anaconda环境方法

File --> setting --> Project --> Project Interpreter --> 右上角⚙ --> Add --> Existing environment --> 选择anaconda3的安装路径(C:\Users\Darren\Anaconda3\python.exe)即可。



2、使用 conda install graphviz 后， import graphviz 仍然报错：

```shell
ModuleNotFoundError: No module named 'graphviz'
```

方法1：

```shell
conda install python-graphviz    #在anaconda promet中安装，可能会下载失败，多试几次就好了
```

方法2：

```shell
pip install graphviz
```

方法1可保证成功。



## 2、数据包在线下载失败的处理方法  

1、在网上下载到对应的数据表，可以在github或CSDN上下载。eg: fashion_minist数据集的下载方法，git clone https://github.com/zalandoresearch/fashion-mnist.git

2、将数据包放到对应的安装路径下，eg：fashion_minist存放到C:\Users\Darren\.keras\datasets\fashion-mnist

3、再次执行就OK了



## 3、jupyter notebook的修改密码方法  

https://www.cnblogs.com/honway/p/9559324.html

修改后密码为：Weng15888J

