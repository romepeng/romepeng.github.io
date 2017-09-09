---
title: git proxy
date: 2017-09-09 16:05:00
---
### git proxy

#### set:
git config --global http.proxy http://127.0.0.1:1080
git config --global https.proxy https://127.0.0.1:1080

#### unset and delelte
git config --global unset http.proxy
git config --global unset https.proxy

npm config delete proxy



