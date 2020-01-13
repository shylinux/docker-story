# {{title "docker"}}

- 官网: https://www.docker.com/
- 开源: https://github.com/docker/docker-ce

{{shell "下载源码" "usr" "install" `wget https://codeload.github.com/docker/docker-ce/zip/master`}}

{{shell "安装服务" "usr" "install" `sudo yum install docker-ce`}}

{{shell "启动服务" "usr" "install" `systemctl start docker`}}

{{shell "查看服务" "usr" `systemctl status docker`}}

## alpine

{{shell "镜像代理" "usr" "install" `sed -i 's/dl-cdn.alpinelinux.org/mirrors.aliyun.com/g' /etc/apk/repositories`}}

{{shell "安装bash" "usr" "install" `apk add bash`}}

{{shell "安装curl" "usr" "install" `apk add curl`}}

