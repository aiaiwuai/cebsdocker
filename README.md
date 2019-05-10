# cebsdocker
## docker and ui
```
git clone git@github.com:aiaiwuai/cebsdocker.git
git submodule init
git submodule update
```  
## branch
med and huicloud 均切换到qwangdev 分支,并和上述文件夹平行,新建平行文件夹db 用于持久化数据

## 安装docker
安装docker(系统不限 win/linux/mac 均可)
确保docker  docker-compose 可用
```
cd xiaohuidocker
docker-compose -f stack.yml up
```
