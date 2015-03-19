# Consul-template nginx image

Basic image containing consul-template and nginx.

## How to use
tag your services with 'http' and they will be proxied.

```

docker run -d -p 80:80 manholsteijn/consul-haproxy -consul consul.service.consul:8500 -template /haproxy.ctmpl:/etc/haproxy/haproxy.cfg:service haproxy reload
```
