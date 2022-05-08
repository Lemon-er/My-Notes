# 在GitHub上将已有文件移动到同一个仓库的另一个文件夹

## 1.将该仓库克隆到本地文件夹：

cmd命令：git clone +仓库地址

例如：git clone https://github.com/nongfulv2/My-Notes.git

![image-20220508183020374](C:\Users\19127\AppData\Roaming\Typora\typora-user-images\image-20220508183020374.png)

## 2.在本地文件夹下进行你想要的操作（比如移动一个文件到另一个文件夹）

注意：此时只是在本地进行了操作，并没有将该操作同步到GitHub账号上，所以就有了下一步

## 3.cmd命令：cd My-Note(进入文件夹)

cmd命令：git add .(意思是把我们要提交的文件的信息添加到暂存区)

cmd命令：git status(查看提交状态)

![image-20220508183738768](C:\Users\19127\AppData\Roaming\Typora\typora-user-images\image-20220508183738768.png)

## 4.git commit -m "a"(主要是将暂存区里的改动给提交到本地的版本库)

![image-20220508184233046](C:\Users\19127\AppData\Roaming\Typora\typora-user-images\image-20220508184233046.png)

## 5.git push(最后一步将本地版本库的分支推送到远程服务器上对应的分支)

![image-20220508184438541](C:\Users\19127\AppData\Roaming\Typora\typora-user-images\image-20220508184438541.png)

大功告成，此时刷新GitHub页面就可以了！

