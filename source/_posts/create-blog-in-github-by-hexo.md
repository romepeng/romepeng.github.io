---
title: hexo在github创建博客
date: 2017-08-05 12:18:24
tags:
---


### hexo 创建博客方法 (github)
E:\hexo\blog\source\_posts( path of *.md)

1. 安装[Node.js](https://nodejs.org/en/)
2. 安装[git for windows](https://git-for-windows.github.io/)
3. 进入“Git Bash”
  $ git config --global user.name "romepeng"
  $ git config --global user.email "romepeng@outlook.com"
4. 安装Hexo：
   $ npm install hexo-cli -g
 5. cd E: ;  mkdir hexo; cd hexo;
 6. hexo init blog
    cd blog
 7. hexo generate
 8. hexo server [http://localhost:4000]
 9. `ssh-keygen -t rsa -C "Github的注册邮箱地址"`
 check: `ssh -T git@github.com`
 10. hexo deploy
     need:  vim _config.yml
			     deploy:
				     type:  git
				     repo: git@github.com:romepeng/romepeng.github.io.git
				     branch: master
				     
			     ` npm install hexo-deployer-git --save`
           
11. new post update
`
      hexo new "My New Post"
      hexo clean
      hexo g
      hexo s
      hexo d
      ( hexo generate --deploy)
     `
12.use my doimanname [see zhihu](https://www.zhihu.com/question/31377141)
      cd \hexo\blog\source  cd.>CNAME  (rr2w.com)

