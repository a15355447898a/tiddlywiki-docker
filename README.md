 # tiddlywiki-docker

---

本项目构建了最新的(截止到2024/4/20)tiddlywiki进了docker,同时是个使用指南

---

## 使用步骤

* 将本项目中的`tiddlywiki-init`和`tiddlywiki-server`下载到你想要存放wiki文件的文件夹下面
* 设置两个脚本的权限
  * `sudo chmod a+x ./tiddlywiki-init`
  * `sudo chmod a+x ./tiddlywiki-server`

* 创建wiki文件夹
  * `./tiddlywiki-init wiki --init server`
    (这里假设你想要用`wiki`文件夹存放wiki,你可以任意重命名)
* 启动docker
  * `./tiddlywiki-serve wiki`
    这里的`wiki`是上一步设置的名称
  * (你可以修改`tiddlywiki-serve`来设置运行的端口,用户名和密码)
    (默认运行在8080端口,登陆的用户名和密码均为`root`)
