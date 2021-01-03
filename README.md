# 简介

网易云音乐 UWP 重打包版，不会自动更新到 Win32 版。

# 下载

Github 源：
[x86 (32位)](https://github.com/JasonWei512/NetEase-Cloud-Music-UWP-Repack/raw/master/%E7%BD%91%E6%98%93%E4%BA%91%E9%9F%B3%E4%B9%90UWP%20%E4%B8%8D%E6%9B%B4%E6%96%B0%E7%89%88%20x86.appx) | 
[x64 (64位)](https://github.com/JasonWei512/NetEase-Cloud-Music-UWP-Repack/raw/master/%E7%BD%91%E6%98%93%E4%BA%91%E9%9F%B3%E4%B9%90UWP%20%E4%B8%8D%E6%9B%B4%E6%96%B0%E7%89%88%20x64.appx) | 
[ARM (未测试)](https://github.com/JasonWei512/NetEase-Cloud-Music-UWP-Repack/raw/master/%E7%BD%91%E6%98%93%E4%BA%91%E9%9F%B3%E4%B9%90UWP%20%E4%B8%8D%E6%9B%B4%E6%96%B0%E7%89%88%20arm.appx)

国内镜像：
[x86 (32位)](https://github.strcpy.cn/JasonWei512/NetEase-Cloud-Music-UWP-Repack/raw/master/%E7%BD%91%E6%98%93%E4%BA%91%E9%9F%B3%E4%B9%90UWP%20%E4%B8%8D%E6%9B%B4%E6%96%B0%E7%89%88%20x86.appx) | 
[x64 (64位)](https://github.strcpy.cn/JasonWei512/NetEase-Cloud-Music-UWP-Repack/raw/master/%E7%BD%91%E6%98%93%E4%BA%91%E9%9F%B3%E4%B9%90UWP%20%E4%B8%8D%E6%9B%B4%E6%96%B0%E7%89%88%20x64.appx) | 
[ARM (未测试)](https://github.strcpy.cn/JasonWei512/NetEase-Cloud-Music-UWP-Repack/raw/master/%E7%BD%91%E6%98%93%E4%BA%91%E9%9F%B3%E4%B9%90UWP%20%E4%B8%8D%E6%9B%B4%E6%96%B0%E7%89%88%20arm.appx)

# 安装说明

1、右键点击 x86 / x64 / ARM 安装包，点击属性，切换到"数字签名"选项卡。双击签名列表中的"esaeten"。在弹出的"数字签名详细信息"窗口中点击"查看证书"，再点击"安装证书"。

2、在"证书导入向导"中：

- "存储位置"选"本地计算机"，下一步。（需要同意UAC权限请求）

- 选择"将所有的证书都放入下列存储"，点击"浏览"，选择"受信任人"，确定，下一步，继续完成证书导入。

3、双击 x86 / x64 / ARM 安装包安装。

4、双击 x86 或 x64 安装包安装。

## UWP 版本无法登录的解决方案

点击发现音乐 → 最新音乐把我喜欢的音乐调出来

从创建的歌单 → 我喜欢的音乐那里点击登录

PS: 应该只支持网易账号和手机号

## 本地回环代理设置

管理员命令行运行：

`checknetisolation loopbackexempt -a -n="1f8b0f94.122165ae053f_kq4t7q4nstjby"`

# 打包方式说明

见 [该 issue](https://github.com/JasonWei512/NetEase-Cloud-Music-UWP-Repack/issues/3#issuecomment-636415035)。