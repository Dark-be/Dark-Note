# Softwares

## Git

* 常用指令

```sh
ssh-keygen -f id_rsa -p                             #更改私钥密码
git pull --allow-unrelated-histories                #忽略历史拉取
```

### SSH

* 使用SSH密钥连接更稳定，详见[Connecting to GitHub with SSH](https://docs.github.com/en/authentication/connecting-to-github-with-ssh)

```sh
ssh-keygen -t ed25519 -C "your_email@example.com"   #密钥需复制到github
eval "$(ssh-agent -s)"                              #启动SSH服务
```




### Work together

* 合作一般遵循以下流程

```sh
git add .
git commit -m "new commit"
git pull
git commit -m "new merge"
git push
```

### Branch

```sh
git branch -m oldName newName                       #本地重命名
----
git branch -m oldName newName                       #远程重命名流程
git push --delete origin oldName
git push origin newName
git branch --set-upstream-to origin/newName
----
git branch --unset-upstream                         #若本地之前已经关联需解除
git branch -u origin/main                           #将本地分支与远程main分支关联，
                                                    #此前最好fetch一次
```

### Remote

```sh
git remote -v                                       #远程仓库地址
git remote show origin                              #查看远程分支信息

```

***

## Docker

* 常用指令

```sh
docker run -it --name=[container name] [image name] #创建容器
docker start [container name]                       #启动容器
docker attach [container name]                      #进入容器
docker exec -it [container name] /bin/bash          #进入容器(伪终端)


```

## CMake

* 

***
