## 提交理由:

为了更加快捷的使用 tf-gpu-keras 环境. 如果每次都从官方pull,耗时太长,要下载3个多G的文件.

## 具体配置:

见dockerfile, 或者dockerhub页面.

## 来源:

[github: gw0](https://github.com/gw0/docker-keras/blob/master/Dockerfile.py3-tf-gpu)

[dockerhub: gw000](https://hub.docker.com/r/gw000/keras)

## 遇到过的问题:

1. 次镜像中python找不到命令,要用python3.

2. 此镜像没有pip.

   装pip:

   ```shell
   wget https://bootstrap.pypa.io/get-pip.py && python3 get-pip.py
   ```

3. 此镜像没有 PIL, 没有 matplotlib. 