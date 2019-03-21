# Win10-python-pytorch-
由于2019年pytorch也发布了支持windows的版本，故安装，并记录下来
1.需要安装anaconda3、cuda10（给gpu加速的）,cudnn和pycharm（编译环境）
2.anaconda3支持的python版本是python3.7，所以pytorch也要安装支持python3.7的版本，在其官网上下载，使用anaconda3提供的python环境安装
3.如果不事先指定国内镜像下载的话会很慢，从而导致有一些文件因为下载时间过长而终止下载，最终导致下载失败，所以要提前弄好国内镜像站：
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/free/
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/main/
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/conda-forge/
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/pytorch/
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/pro/
4.下载后运行可能会出现跟numpy相关的错误，需要先把numpy全部卸载：conda uninstall numpy，再重新下载：pip3 install numpy，即可
