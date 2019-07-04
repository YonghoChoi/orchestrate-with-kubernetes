# 워드프레스 구축하기

## secret 등록
1. tls 인증 파일 secret에 등록
```
kubectl create secret generic tls-certs --from-file tls/
```

## config 등록
1. nginx 설정을 configMap에 등록
```
kubectl create configmap nginx-proxy-conf --from-file nginx/proxy.conf
```