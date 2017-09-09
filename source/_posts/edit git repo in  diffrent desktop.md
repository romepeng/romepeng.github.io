---
title: edit git repo in many desktop
date: 2017-09-09 17:00:24
---
#### edit git repo in  diffrent desktop

## method:
1.  create a new repo on github ;
2.  git clone https://github.com/romepeng/windpyplus.git
3.  edit the project
4.  git add .
5.  git commit -m ' log';
6.  git push origin master ;
if github have files, error output: now
7. git pull origin master;
then, do  item 6.

push error: src refspec master does not match any;
method:
touch README
git add README
git commit -m 'slove error'
git push origin master

add remote repo:
git remote add origin https://github.com/romepeng/windpyplus.git
check:
git remote -v

so:
项目先clone下， edit or add or delete 。提交前， pull一下， 保持与服务器的版本一致， add. 后，commit提交，写说明， 再push上去。



 