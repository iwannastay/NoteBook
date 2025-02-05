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


git config --global http.sslverify false
git config --global credential.helper store
git config --global push.default matching
git config --global http.postBuffer 2M

git config --global http.proxy "http://xxxx"
git config --global https.proxy "https://xxxx"
```