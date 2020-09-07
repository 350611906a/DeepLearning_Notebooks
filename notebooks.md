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



## 4、将所有结果保存到github上  

步骤：

- 本地新建一个文件夹

- 进入后，右击 --> Git Bash Here --> 初始化`git init`（会出现master，表示主分支），--> ls -a --> 可以查看到./git，表示成功。

- 查看远程信息

  git remote -v

- 将本地仓库与远程仓库关联

  git remote add origin https://github.com/350611906a/DeepLearning_Notebooks

- 将远程仓库clone到本地

  git clone https://https://github.com/350611906a/DeepLearning_Notebooks

  clone下来之后，远程连接就建立了，因为clone下来的仓库已经有了.git文件。

- 本地修改后，上传到本地仓库

  git commit -a -m "日志"

- 上传到github

  git push origin master



## 5、github出现错误的解决方法  

1、报错：

```shell
 git clone https://github.com/350611906a/DeepLearning_Notebooks
Cloning into 'DeepLearning_Notebooks'...
fatal: unable to access 'https://github.com/350611906a/DeepLearning_Notebooks/': OpenSSL SSL_connect: SSL_ERROR_SYSCALL in connection to github.com:443
```

解决方法：

在github项目在本地的根目录下打开git命令行，执行如下命令：

```shell
git config --global --unset http.proxy
```





