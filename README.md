# nginx.conf
打开conf/nginx.conf

把user改成你服务器的用户名

server对象就是服务器的配置

listen为端口

主要修改locatino对象

```javascript
location / {
    root   index.html所在的目录;
    index  index.html index.htm;
}
```

#启动
```shell
sudo /nginx-sbin-path -p /project-path -c /conf-path 
```
如：
```shell
sudo /usr/local/openresty/nginx/sbin/nginx -p /work/openresty-test/ -c conf/nginx.conf
```

#停止
```shell
sudo /nginx-sbin-path -p /project-path -c /conf-path -s stop
```
如:
```shell
sudo /usr/local/openresty/nginx/sbin/nginx -p /work/openresty-test/ -c conf/nginx.conf -s stop
```# openresty-test
