# deploymentOnline
部署NodeJs上线步骤
## 打开http://brew.sh/index.zh-cn.html 即homebrew的官网 在mac上执行安装命令
1. `brew search nginx` `brew install nginx` 查看本地计算即是否存在nginx，如果不存在执行后面的安装命令
2. `brew info nginx` `nginx -v` 查看nginx信息
3. `nginx` 启动nginx服务(默认是8080端口) 也可以使用 sudo brew services start nginx启动
4. 如果提示80端口被使用 首先`nginx -s stop` 然后再重新启动`nginx`
5. 关闭 `sudo brew services stop nginx / nginx`
6. `nginx -s reload`和`nginx -s stop`
8. 打开nginx具体安装目录 ，查看配置文件  `/usr/local/etc/nginx`--nginx.conf
9. 配置nginx.conf文件
10. http upstream模块--配置多台服务器实现负载均衡
# nginx.conf 配置文件
