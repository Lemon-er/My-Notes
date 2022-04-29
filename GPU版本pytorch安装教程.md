## 第一步：下载cuda和cudnn

1.首先要查看自己电脑英伟达gpu的版本从而下载相应的cuda版本，有两种方法查看：

①打开cmd命令行：输入nvcc --version

例如我的版本就是11.6的

![image-20220428203055134](https://img-blog.csdnimg.cn/0db1c0b7a62c4afa9d3e8fd6d1efecef.png)

②进入控制版面-->硬件和声音-->NVIDIA控制面板-->帮助点系统信息-->点击组件即可看到

2.cuda下载地址：[CUDA Toolkit Archive | NVIDIA Developer](https://developer.nvidia.com/cuda-toolkit-archive)

下载对应版本的cuda即可

![image-20220428205042717](https://img-blog.csdnimg.cn/028e31ee3eab4b77b6c636995512e664.png)



选择相应的版本下载即可：

![image-20220428205158809](https://img-blog.csdnimg.cn/820b6837b843482a8147359bc7446a82.png)

3.下一步下载cudnn，链接：

[cuDNN Archive | NVIDIA Developer](https://developer.nvidia.com/rdp/cudnn-archive#a-collapse51b)

选择对应版本：

![image-20220428205431064](https://img-blog.csdnimg.cn/ae3e33b748de41619422d8946b1266b7.png)

点击后要注册或登录英伟达账户才能下载，很麻烦，这里可以右键复制下载链接到迅雷直接下载更方便

## 第二部：安装CUDA、cudnn和配置环境变量

1.安装cuda:

双击运行下载好的cuda的exe文件，安装时不要乱改路径，一路OK，同意等待就好了

![image-20220428210501837](https://img-blog.csdnimg.cn/2144312e882f47d6b3b2370966c2bae3.png)

选择自定义安装

![image-20220428231207261](https://img-blog.csdnimg.cn/ae6577a24ada4410babada1c1a274e3f.png)

后面的路径也不要改，直接安装即可。安装完成后cmd命令行输入“nvcc -V”，查看是否成功

例如这样就可以了：

![image-20220428231602945](https://img-blog.csdnimg.cn/3aba23da68ab488b8cbc9e9024f4318b.png)

2.轮到cudnn了

将下载好的压缩包解压后重命名里面的文件名为“cudnn”，然后再复制到该路径下

![image-20220429123837845](https://img-blog.csdnimg.cn/d6a970ee5eed49099632100f1c125de8.png)

接着不要忘记配置环境变量（我曾两度忘记）

找到控制面板-->系统和安全-->系统（或进入我的电脑，右键选择属性）选高级系统设置找到环境变量

![image-20220429124446410](https://img-blog.csdnimg.cn/3492ec40d50844beb51eed095c7ca0fa.png)

进入path这个变量

![image-20220429124743727](https://img-blog.csdnimg.cn/51165c48b2934c4b9c2d53c5242ad319.png)

新建，添加这两个路径即可

C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v11.3\cudnn\bin
C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v11.3\extras\CUPTI\lib64



![image-20220429124804633](https://img-blog.csdnimg.cn/567e48b2009a44e9a545c5f8b483bb67.png)

## 第三步：下载cudatoolkit和GPU版本的[pytorch](https://so.csdn.net/so/search?q=pyTorch&spm=1001.2101.3001.7020)、pytorchvision

1.cudatoolkit下载链接：[Start Locally | PyTorch](https://pytorch.org/get-started/locally/)

选择对应版本的，复制命令取cmd里执行即可（第一次有部分包安装失败可以多尝试几次）

![image-20220429131700490](https://img-blog.csdnimg.cn/bbfc65781087475d8192d17d6f8ec95d.png)

下载完在cmd里输入“conda list”查看，有cudatoolkit即可

![image-20220429141519568](https://img-blog.csdnimg.cn/912d7ccd79854d45be80985d997876d9.png)

2.GPU版本的[pytorch](https://so.csdn.net/so/search?q=pyTorch&spm=1001.2101.3001.7020)、pytorchvision的下载链接：https://download.pytorch.org/whl/torch_stable.html

里面的文件是cpu开头的是CPU版本，cu才是我们要下的gpu版本

我的cuda版本比较高，下的是1.9.1的torch版本（cuda版本对应的具体torch版本可以百度）；我的python是3.9的，对应的是后面的39；区别win和linux

![image-20220429140424712](https://img-blog.csdnimg.cn/466577dce28c499ebe4392e4a5415efd.png)

torchvision也一样

![image-20220429140540967](https://img-blog.csdnimg.cn/4cfc65c3ed644e3e9272be95d8c91376.png)

下载好后放在同一个目录下，在cmd下进入这个路径，pip install +“文件名“（注意有引号）

(cmd进入指定目录的方法：①输入”盘符+  :  “②输入”cd+空格+指定路径+回车“)

查看检验方法：输入命令：pip list,看到一下就好了

![image-20220429150559586](https://img-blog.csdnimg.cn/b2349bd5b524482b9dcd44d800c6ec79.png)

![image-20220429152455264](https://img-blog.csdnimg.cn/a0e7cde3615c40d8951013229d37f89a.png)

Ture说明成功了。
