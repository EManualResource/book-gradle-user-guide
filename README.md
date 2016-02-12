## {book-BookName}

### 使用

#### 新建一文档

```shell
# clone文档模板
$ git clone git@github.com:EManual/book-boilerplate.git {book-BookName}
$ cd {book-BookName}

# 注意，此处submodule必须是https协议，不能是ssh协议
$ git submodule add https://github.com/user/repo.git ./source 

# [可选步骤]更改文件的配置
$ vim Makefile
```

### 维护文档

```shell
# [可选步骤]首次下载
$ git clone --recursive git@github.com:EManualResource/{BookName}.git

# 更新source
$ make update-source

# 构建
$ make

# 本地预览，访问： http://localhost:8000
$ make serve
```
