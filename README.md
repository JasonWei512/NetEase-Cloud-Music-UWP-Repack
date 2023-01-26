# 简介

网易云音乐 UWP 重打包版，不会自动更新到 Win32 版。

# 下载

[下载地址](https://github.com/JasonWei512/NetEase-Cloud-Music-UWP-Repack/archive/refs/heads/master.zip)

单独安装包：[x86 (32位)](https://github.com/JasonWei512/NetEase-Cloud-Music-UWP-Repack/raw/master/%E7%BD%91%E6%98%93%E4%BA%91%E9%9F%B3%E4%B9%90UWP%20%E4%B8%8D%E6%9B%B4%E6%96%B0%E7%89%88%20x86.appx) | 
[x64 (64位)](https://github.com/JasonWei512/NetEase-Cloud-Music-UWP-Repack/raw/master/%E7%BD%91%E6%98%93%E4%BA%91%E9%9F%B3%E4%B9%90UWP%20%E4%B8%8D%E6%9B%B4%E6%96%B0%E7%89%88%20x64.appx) | 
[ARM (32位)](https://github.com/JasonWei512/NetEase-Cloud-Music-UWP-Repack/raw/master/%E7%BD%91%E6%98%93%E4%BA%91%E9%9F%B3%E4%B9%90UWP%20%E4%B8%8D%E6%9B%B4%E6%96%B0%E7%89%88%20arm.appx)

# 安装说明

1. 右键点击 x86 / x64 / ARM 的 ```appx``` 安装包，点击属性，切换到"数字签名"选项卡。双击签名列表中的"esaeten"。在弹出的"数字签名详细信息"窗口中点击"查看证书"，再点击"安装证书"。

2. 在"证书导入向导"中：

- "存储位置"选"本地计算机"，下一步。（需要同意UAC权限请求）

- 选择"将所有的证书都放入下列存储"，点击"浏览"，选择"受信任的根证书颁发机构"，确定，下一步，继续完成证书导入。

3. 双击 x86 / x64 / ARM 的 ```appx``` 安装包安装。

# 无法登录的解决方案

请选择以下其中一种方法：

**[方法一（推荐）：](https://www.bilibili.com/read/cv9556360/)**

1. 点击 左下角“未登录”头像 → 关于网易云音乐，来到关于界面

2. 对界面右上角的网易云音乐 Logo 连续单击5下，然后迅速右击，会弹出调试对话框（如果不行则多试几次）

3. 将对话框中的服务地址 ```http://music.163.com``` 中的 ```http``` 改为 ```https```，即改为 ```https://music.163.com```，然后确认

4. 重启应用后登录

- [查看动图演示](https://i0.hdslb.com/bfs/article/5a5c6a3e97209bdc94e9a8440c7a4abff93fcb72.gif)

**方法二：**

1. 点击 发现音乐 → 最新音乐，此时“我喜欢的音乐”会出现在应用左栏

2. 点击 创建的歌单 → 我喜欢的音乐 → “未登录”头像，然后登录

- 注：应该只支持网易账号和手机号

**方法三：**
部分账号会提示需要验证，但是UWP版本是输不了验证码的...

解决办法是使用第三方登录，比如QQ登录，方可正常使用！

# 进阶：本地回环代理设置

（如果你不知道这是做什么的，那么请忽略这一项）

管理员命令行运行：

`checknetisolation loopbackexempt -a -n="1f8b0f94.122165ae053f_kq4t7q4nstjby"`


# 已知问题

在 Windows11 22H2 版本之上，无法下载音乐，见 [该 issue](https://github.com/JasonWei512/NetEase-Cloud-Music-UWP-Repack/issues/24) 。

# 打包方式说明

见 [该 issue](https://github.com/JasonWei512/NetEase-Cloud-Music-UWP-Repack/issues/3#issuecomment-636415035)。
