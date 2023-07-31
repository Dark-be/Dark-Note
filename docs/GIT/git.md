## Git
[My Github]()
***
#### SSH
* 使用SSH密钥连接更稳定，详见[Connecting to GitHub with SSH](https://docs.github.com/en/authentication/connecting-to-github-with-ssh)

#### Common command
```sh
ssh-keygen -f id_rsa -p   #更改私钥密码
git help                  #获取帮助
```
#### Work together
* 合作一般遵循以下流程
```sh
git add .
git commit -m "new commit"
git pull
git commit
git push
```
