#### 1. issuecode

> git代码发布工具，增量更新工具

###### 安装:

    wget --no-check-certificate http://t.cn/RLV8yDH  -O /usr/bin/issuecode
    chmod +x /usr/bin/issuecode

###### 参数说明：
 
* -v  从git版本库里导出的版本，如为空则为最近一次提交的修改，导出文件为zip压缩包
 
* -s  scp上传的服务器，该参数依赖.ssh文件夹下的config配置
 
* -l  上传到-s参数的服务器后，是否直接登录服务器

###### 使用方法：

进入到相应的git项目根目录，执行下面命令:

    issuecode #无任何参数, 将导出最新一次提交的修改
    issuecode -v 485642b #将导出从485642b版本以后修改的所有文件

- - -