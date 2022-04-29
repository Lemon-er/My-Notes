#1.创建仓库
仓库是存储想法、资源甚至与他人共享和讨论的地方。（记笔记的地方）
1.在任何页面的右上角，使用  下拉菜单选择 New repository（新建仓库）。
![](https://img-blog.csdnimg.cn/img_convert/4f77975ae4c3af632b9e939156969186.png)
2.在 Repository name（存储库名称）框中，输入 hello-world。

3.在 Description（说明）框中，编写简短说明。

4.选择 Add a README file（添加 README 文件）。

5.选择您的存储库是公有还是私有。

6.单击 Create repository（创建仓库）
![](https://img-blog.csdnimg.cn/img_convert/a5a2e91506ff00387a4f5ec2b6f794da.png)








#2.创建一个main的分支
分支是什么呢？我的理解就是main好比是一张正式的数学试卷，创建的分支就是带有做题时间和为什么这么做这道题的可以打草稿的副本数学试卷。

具体怎么做呢？如下：

1.单击 hello-world 存储库的 Code（代码）选项卡。
2.单击其中显示 main 的文件列表顶部的下拉列表。
![](https://img-blog.csdnimg.cn/img_convert/ee2c56316899186e2dd8e52e521736c1.png)

3.在文本框中键入分支名称 readme-edits。
4.单击 Create branch: readme-edits from main（创建分支：从 main 创建 readme-edits）。
![](https://img-blog.csdnimg.cn/099d0dc996ba4113a2d4aeecd5443750.png?x-oss-process=image/watermark,type_d3F5LXplbmhlaQ,shadow_50,text_Q1NETiBA5Yac5aSrbHYy,size_15,color_FFFFFF,t_70,g_se,x_16)
5.此时您有两个分支：main 和 readme-edits。 现在，它们看起来完全相同。 接下来，您将向新分支添加更改。


#3. 提交更改
1.在您创建的 readme-edits 分支下，单击 README.md 文件。

2.单击 🖊 编辑文件，输入“这是记录日常学习笔记用的仓库！”

3.在编辑器中，编写一些关于您自己的内容。 尝试使用不同的 Markdown 元素。

4.在 Commit changes（提交更改） 框中，编写描述更改的提交消息。

5.单击 Commit changes（提交更改）。
![](https://img-blog.csdnimg.cn/ac63147eb1534031a304439d6642268e.png?x-oss-process=image/watermark,type_d3F5LXplbmhlaQ,shadow_50,text_Q1NETiBA5Yac5aSrbHYy,size_20,color_FFFFFF,t_70,g_se,x_16)

 这样就把分支中的readme文件编辑好了，这些更改将仅适用于 readme-edits 分支上的 README 文件，所以这个分支现在包含不同于 main 的内容。

 ![](https://img-blog.csdnimg.cn/26d57e9166ed4a8d9b147c0476bbb58e.png?x-oss-process=image/watermark,type_d3F5LXplbmhlaQ,shadow_50,text_Q1NETiBA5Yac5aSrbHYy,size_20,color_FFFFFF,t_70,g_se,x_16)

4. 合并到main上+拉取请求
现在，您在 main 以外的分支中进行了更改，可以打开拉取请求。

拉取请求是 GitHub 上协作的核心。 打开拉取请求后，可以提出更改，要求某人审查和提取您的贡献并将其合并到其分支中。 拉取请求显示两个分支中内容的差异。 变化、增减以不同的颜色显示。

只要进行提交，便可打开拉取请求并开始讨论，即使在代码完成之前亦可。

通过在拉取请求消息中使用 GitHub 的 @提及功能，您可以向特定人员或团队请求反馈，无论他们近在大厅还是远在 10 个时区之外。

您甚至可以在自己的存储库中打开拉取请求并自行合并。 这是在处理大型项目之前了解 GitHub 流程的好方法。
1.单击 hello-world 存储库的 Pull requests（拉取请求）选项卡。

2.单击 New pull request（新拉取请求）。

3.在 Example Comparisons（示例比较）框中，选择您创建的分支 readme-edits 以与 main（原始分支）进行比较。

4.在 Compare（比较）页面上的差异中查看您的更改，确保它们是您要提交的内容。

5.单击 Create pull request（创建拉取请求）。

6.为拉取请求指定一个标题，并写下更改的简要说明。 您可以包含表情符号以及拖放图像和 gif。

7.（可选）在标题和说明右侧，单击 Reviewers（审查者）旁边的 。 单击 Assignees（受理人）、Labels（标签）、Projects（项目）或 Milestone（里程碑）以将这些选项添加到您的拉取请求。 您不需要添加任何内容，但这些选项提供了使用拉取请求进行协作的不同方式。 更多信息请参阅“关于拉取请求”。

8.   单击 Create pull request（创建拉取请求）。

![](https://img-blog.csdnimg.cn/b95c5f7624224d5c9b1e2c8e9a246330.png?x-oss-process=image/watermark,type_d3F5LXplbmhlaQ,shadow_50,text_Q1NETiBA5Yac5aSrbHYy,size_16,color_FFFFFF,t_70,g_se,x_16)





在最后一步中，您将 readme-edits 分支合并到 main 分支中。 合并拉取请求后，readme-edits 分支上的更改将合并到 main。

有时，拉取请求可能会引入与 main 上现有代码冲突的代码更改。 如果存在任何冲突， GitHub 将提醒您有关冲突代码的信息，并防止合并，直到冲突解决为止。 您可以进行解决冲突的提交，也可以使用拉取请求中的注释与团队成员讨论冲突。

在本演练中，应该没有任何冲突，因此您已准备好将分支合并到主分支中。

1.单击 Merge pull request（合并拉取请求），将更改合并到 main。
2.单击 Confirm merge（确认合并）。 您将收到一条消息，指出请求已成功合并且请求已关闭。
3.单击 Delete branch（删除分支）。 现在，您的拉取请求已合并，并且您的更改位于 main 上，您可以安全地删除 readme-edits 分支。 如果要对项目进行更多更改，可以随时创建新分支并重复此过程。
![](https://img-blog.csdnimg.cn/4eb2351c5a674690b5e085b290b82b01.png?x-oss-process=image/watermark,type_d3F5LXplbmhlaQ,shadow_50,text_Q1NETiBA5Yac5aSrbHYy,size_20,color_FFFFFF,t_70,g_se,x_16)

总结： 

已经学会并完成了如下功能，上手试试吧 

创建了一个开源仓库
启动并管理了新的分支
更改了文件并将这些更改提交到 GitHub
打开并合并了拉取请求
​
