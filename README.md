# cebsdocker
## docker and ui
```
mkdir ./somedir
cd ./somedir
git clone git@github.com:aiaiwuai/ui.git www
git clone git@github.com:aiaiwuai/xiaohuidocker.git xiaohuidocker
git clone git@github.com:Baxianxiahai/huicloud.git
cd huicloud
git checkout qwangdev
cd ../
git clone git@github.com:Baxianxiahai/med.git
cd med
git checkout qwangdev
cd ../
mkdir ./db
```  
## 安装docker
安装docker(系统不限 win/linux/mac 均可)
确保docker  docker-compose 可用
```
cd xiaohuidocker

docker-compose -f stack.yml up
docker-compose -f stack.yml [up|restart] [tup|hst|ui....]
docker-compose -f stack.yml logs -f tup
```
## 初始化hst数据
docker exec -it hst /bin/bash
python PkgUt/_UtEntry.py
## 重启tup
docker-compose -f stack.yml up tup

## 端口
- 数据库管理
- 127.0.0.1:8088
- UI
- 127.0.0.1:7589
- MQTT WEB 管理
- 127.0.0.1:18083
