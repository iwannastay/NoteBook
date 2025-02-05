# git配置

## 查看
```shell
git config --system --list
git config --global --list
git config --local --list
```

## 认证
```shell
# ssh public key
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"

# personal token 
git config --global credential.helper manager-core


```

## 鉴权
```shell


git config --local http.sslverify false
git config --local credential.helper store
git config --local push.default matching
git config --local http.postBuffer 2M

git config --local http.proxy "http://xxxx"
git config --local https.proxy "https://xxxx"
```