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
```
