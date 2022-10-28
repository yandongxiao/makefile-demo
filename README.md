本项目主要拷贝了 https://github.com/marmotedu/iam 项目中关于 Makefile 相关的内容。

```bash
# 拷贝的额内容
cp -r Makefile scripts build githooks /tmp/makefile-demo

# 修改 Makefile，忽略 gen.run target
# ignore gen.run

# 修改 Makefile 中该字段的内容
ROOT_PACKAGE=github.com/yandongxiao/makefile-demo

# 修改 scripts/make-rules/image.mk，调整容器镜像的前缀。基础镜像
REGISTRY_PREFIX ?= yandongxiao
BASE_IMAGE = centos:centos8

# 需要事先打出 tag
# docker images
REPOSITORY                TAG               IMAGE ID       CREATED              SIZE
yandongxiao/app-amd64     v0.1.0            442e8c97c1bc   8 seconds ago        231MB
```

