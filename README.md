# 常用git命令

* 提交分支baozi_v1.1到远程服务
>git push origin baozi_v1.1
* 切换到android分支
>git checkout android
* 合并分支baozi_v1.1到当前分支
>git merge baozi_v1.1
* 创建分支baozi_dev3.0.0
>git branch baozi_dev3.0.0
* 拉取分支baozi_v1.1
>git pull origin baozi_v1.1
* 获取新创建的分支
>git fetch 获取新创建的分支

* 在本地项目所在目录按以下步骤操作
>git init<br>
git add README.md<br>
git commit -m "first commit"<br>
git remote add origin https://github.com/baoziguo/SeeMovie.git<br>
git pull origin master<br>
git push -u origin master<br>

* 但到第四步出现了以下问题

>Administrator@USER-20140819FI /d/git_dir/git_play_repo (master)
$ git remote add origin https://github.com/baoziguo/SeeMovie.git
fatal: remote origin already exists.
* 解决办法如下：

>1、先输入$ git remote rm origin<br>
2、再输入$ git remote add origin git@github.com:dengzhaotai/vlc_play.git 就不会报错了！
