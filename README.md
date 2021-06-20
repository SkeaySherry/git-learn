#### GIT第二天

##### 本地和远程仓库相关联

```
#在项目目录下新建一个文件(建议是README.md)
git init 
git add
git commit -m "first commit"
#git remote add这一步是做关联
git remote add origin https://github.com/SkeaySherry/git-learn.git
git remote add origin git@github.com:SkeaySherry/git-learn.git
#提交到网络仓库,-u及后面的代码,只需要第一次推送的时候执行
git push -u origin master
```

#### HTTPS协议和SSH协议的区别

- HTTPS协议 -提交的时候会验证用户信息(验人)
- SSH协议 -需要进行配置, 配置好后不需要验证用户信息(验机器)