# NGINX+ as Reverse Proxy deployment in K8S using ConfgMaps

1. Download your jwt token, cert and key from https://my.f5.com
2. From same folder use following command to get tag list of images available at NGINX private registry, this applies to base image
```
curl -s https://private-registry.nginx.com/v2/nginx-plus/base/tags/list --key ./nginx-repo.key --cert ./nginx-repo.cer  | jq
```
``Note:`` For image with agent and rootless image please [follow](https://docs.nginx.com/nginx/admin-guide/installing-nginx/installing-nginx-docker/#pulling-the-image) 

4. Create config Maps
5. Create you
