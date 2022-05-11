### token

http://www.bubuko.com/infodetail-3811638.html
https://www.cnblogs.com/sober-orange/p/git-token-push.html



https://blog.csdn.net/FatalFlower/article/details/119717823
https://blog.csdn.net/rzleilei/article/details/119702463
https://blog.csdn.net/qq_22823581/article/details/119827438
https://www.jianshu.com/p/f94ab86d49c8


## 常用命令
切换到git项目，使用下面的命令清空本地存储的账号密码。
git config --local credential.helper ""
git config --global credential.helper store



git remote set-url origin https://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@github.com/feirenraoyuan/linux.git
git clone https://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@github.com/feirenraoyuan/linux.git


OpenSSL SSL_read: Connection was reset, errno 10054
输入 git config --global http.sslVerify "false" ，解除SSL验证；


===========================
git config user.name
git config user.email

修改，用户名，邮箱
git config --global user.name "xxx"
git config --global user.email "xxx"

移除仓库，重新添加
git remote rm origin
git remote add origin https://github.com/XXX

2.解除SSL认证
在 Git Bash 中输入以下命令：
git config --global http.sslVerify "false"

3.更新 DNS 缓存
cmd 窗口输入

ipconfig /flushdns





##########



