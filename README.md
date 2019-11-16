```
参考：https://github.com/zacker330/jenkins-install-plugins-shell.git
对其中的shell脚本做细微修改:
当lock文件存在时，不在重新创建目标插件对应的lock目录
shell中基于jenkins官网镜像固定了REF、JENKINS_WAR_PATH的取值,必要时请注释掉


git clone https://github.com/ct1104/jenkins-plugins-batch-install-update.git
cd jenkins-install-plugins-shell
chmod +x install-plugins.sh jenkins-support
export JENKINS_WAR_PATH=<Jenkins war文件的路径>
export REF=<Jenkins中plugins文件夹路径>     路径包含plugins
./install-plugins.sh < plugins.txt
```

plugins.txt:

```
ansible:1.0
powershell:1.3
```
