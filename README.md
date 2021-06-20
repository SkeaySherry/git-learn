# GIT第二天

### 本地和远程仓库相关联

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

### HTTPS协议和SSH协议的区别

- HTTPS协议 -提交的时候会验证用户信息(验人)

- SSH协议 -需要进行配置, 配置好后不需要验证用户信息(验机器)

  

  ### SSH的配置

  ##### 生成key

  1.打开Git命令行

  2.

  ```3.zai
  #生成key的命令,注意,邮箱地址要填写github登录的邮箱
  ssh-keygen -t rsa  -b 4096 -C "2214151129@qq.com"
  ```

  3.在C:\Users\用户名\\.ssh下查看生成的key文件id_rsa是私钥文件,id_rsa.pub是公钥文件

  ##### 添加密钥到Github

  1. 复制刚生成的id-rsa.pub文件的内容

  2. 在github中点击右上角自己的头像,然后点击settings

  3. 点击右侧菜单栏中的SSH and GPG keys

  4. 点击右侧new SSH key 按钮

  5. 将复制的公钥内容放到key中,title中建议输入电脑名称,然后点击添加

  6. 在git命令行中输入ssh -T git@github.com, 显示Hi SkeaySherry! You've successfully authenticated, but GitHub does not provide shell access. 则配置成功

     

     ### 更换远程仓库地址

     1. git remove rm origin -删除已经配置的网络仓库地址

     2. git remove add origin ssh地址

        

        ### 提交步骤

        1. git add .

        2. git commit -m "message"
        3. git push 

     