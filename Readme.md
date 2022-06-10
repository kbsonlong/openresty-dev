
```bash
$ git clone https://github.com/kbsonlong/openresty-dev.git
$ cd openresty-dev
$ docker run -d --name openresty_test openresty/openresty
$ docker cp openresty_test:/usr/local/openresty/nginx/conf/nginx.conf `pwd`/openresty/nginx/
$ docker cp openresty_test:/etc/nginx/conf.d/default.conf `pwd`/openresty/nginx/conf.d/
$ docker rm -i openresty_test
```