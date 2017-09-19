## ab -c 100 -n 100000

+ OpenResty echo: 17k rps

+ OpenResty lua: 15.5k rps

+ OpenResty file: 14.9k rps
+ nginx 403: 14.7k rps

+ spirit: 9k rps
+ micro: 8.7k rps
+ njs http: 8.4k rps

+ expressjs: 5k rps

+ java: 1.6k rps
+ java+mongodb: 1.2k rps


## With Keep Alive:

  + nginx 404/403: 50k rps WOW !
  + OpenResty lua: 42k rps  WOW !!!

  + OpenResty file: 29.7k rps
  + OpenResty echo: 17.6k rps


### Notes

http -> nginx -> proxy_pass -> proxy_cache -> memcache zone -> memcached -> redis cluster -> openresty redis module


## OpenResty lua

 + ngx.say 15.5k rps
