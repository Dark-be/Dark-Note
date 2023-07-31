## Git
[My Github]()
***
#### SSH
* 使用SSH密钥连接更稳定，详见[Connecting to GitHub with SSH](https://docs.github.com/en/authentication/connecting-to-github-with-ssh)
```sh
ssh-keygen -t ed25519 -C "your_email@example.com"   #密钥需复制到github
eval "$(ssh-agent -s)"                              #启动SSH服务
```
#### Common command
```sh
ssh-keygen -f id_rsa -p                             #更改私钥密码
git help                                            #获取帮助
git pull --allow-unrelated-histories                #忽略历史拉取
```
#### Work together
* 合作一般遵循以下流程
```sh
git add .
git commit -m "new commit"
git pull
git commit -m "new merge"
git push
```
#### Pages
```sh
docsify serve docs                                  #启动本地网页生成
```