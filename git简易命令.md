##### 1.      git init                                                       //   初始化

##### 2.       git add .                                                     // 添加文件到暂存区

##### 3.      git commit -m "提交文件"                 // 提交文件到暂存区

##### 4.    git remote add origin git@github.com:wangjiax9/beautifulDay.git         //关联gitbug仓库

###### 5.   git push -u origin master   // 上传本地代码



### 扩展

1. **绑定用户 **

​                  git config --global user.name ''nelyo-nc9"

​                 git config --global user.email ''nelyo@foxnail.com"

2.**为Github账户设置SSH key**

```
加密传输的算法有好多，git使用rsa，rsa要解决的一个核心问题是，如何使用一对特定的数字，使其中一个数字可以用来加密，而另外一个数字可以用来解密。这两个数字就是你在使用git和github的时候所遇到的public key也就是公钥以及private key私钥。

其中，公钥就是那个用来加密的数字，这也就是为什么你在本机生成了公钥之后，要上传到github的原因。从github发回来的，用那公钥加密过的数据，可以用你本地的私钥来还原。

如果你的key丢失了，不管是公钥还是私钥，丢失一个都不能用了，解决方法也很简单，重新再生成一次，然后在github.com里再设置一次就行
```

- 生成ssh key-------------`ssh-keygen -t rsa -C “6215048wjl@163.com`”   来生成。
- 显示ssh公钥的内容： `cat ~/.ssh/id_rsa.pub` 

3.  **为github账号配置ssh key**

   