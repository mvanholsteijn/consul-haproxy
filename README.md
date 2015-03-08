# Consul-template haproxy image

Basic image containing consul-template and haproxy.

## How to use
```
docker run -d -p 80:80 cargonauts/consul-haproxy -consul consul.service.consul:8500 -template /haproxy.ctmpl:/etc/haproxy/haproxy.cfg:service haproxy restart
```
