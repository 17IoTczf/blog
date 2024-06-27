# git版本回退-git push后撤销
[doc]
## 1.git log
根据结果，复制将要**回退至**的**commmit号**
## 2.git reset --soft commmit号
- 命令中的版本号就是1中复制的commmit号
- 如果执行不成功，注意命令中是否在单词和数字之间加了空格
## 3.git log 
- 看效果，如果最新commit号已经回退到想要回退的版本就成功了
- 如果不成功，2执行出错
## 4.git push origin 分支名字 --force
- 分支名字一般是main
- 命令是将最新的commit强制推到远程仓库，也就是git push 之后撤销
- git 版本回退的一种方式

