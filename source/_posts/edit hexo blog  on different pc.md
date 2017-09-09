
---
title:  use hexo on different desktop
date: 2017-09-09 17:14:24
---
####   edit hexo blog  on different pc
#### 思路：
一个分支来存放Hexo生成的网站原始文件（hexo）， 另一个分支来存放生产的静态网页。

流程：
1. 创建仓库，http://CrazyMilk.github.io；
2. . 创建两个分支：master 与 hexo；
3. . 设置hexo为默认分支（因为我们只需要手动管理这个分支上的Hexo网站文件）；
4.  使用git clone git@github.com:CrazyMilk/CrazyMilk.github.io.git拷贝仓库；
5.   在本地http://CrazyMilk.github.io文件夹下通过Git bash依次执行npm install hexo、hexo init、npm install 和 npm install hexo-deployer-git（此时当前分支应显示为hexo）;
6.   修改_config.yml中的deploy参数，分支应为master；
7.   依次执行git add .、git commit -m "..."、git push origin hexo提交网站相关的文件；
8.   执行hexo g -d生成网站并部署到GitHub上。

作者：CrazyMilk
链接：https://www.zhihu.com/question/21193762/answer/79109280
来源：知乎

