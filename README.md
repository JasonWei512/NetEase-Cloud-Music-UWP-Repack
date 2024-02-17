# 简介

经典的**网易云音乐UWP**重打包版，可以与最新官方版共存。

此版本合并了100和400尺寸图形资源，并首次修复了Win11系统下的文件访问权限问题。


# 下载

下载安装包：
[x64 (64位)](https://github.com/exp-3/Cloud-Music-UWP-Repacked/raw/main/cloudmusic.uwp_repack_x64.appx) | 
[x86 (32位)](https://github.com/exp-3/Cloud-Music-UWP-Repacked/raw/main/cloudmusic.uwp_repack_x86.appx) | 
[arm32](https://github.com/exp-3/Cloud-Music-UWP-Repacked/raw/main/cloudmusic.uwp_repack_arm.appx)

下载工具包： 
[非必要,按需下载](https://github.com/exp-3/Cloud-Music-UWP-Repacked/archive/refs/heads/tools.zip)


# 安装

由于Windows只允许安装来自**微软商店**或者**企业开发者**的appx/msix软件包，<br />
所以我们需要先安装**自签名证书**来伪装成企业开发者，才能安装第三方软件包。

请选择以下其中一种方法：

#### 方法一：

1. 下载工具包，务必解压缩所有文件 (不要在压缩包内打开)

2. 打开```一键安装根证书.bat```，根据提示操作即可

3. 当显示内容包含 ```证书 "patched" 添加到存储``` 或者 ```证书 "patched" 已经在存储中``` 说明安装成功

> 某些杀毒软件可能会将此工具误报为病毒，您可能需要暂时关闭杀毒软件或者添加白名单才能使用。或者也可以考虑使用下面的方法二。

#### 方法二：

1. 下载 [证书文件](https://github.com/exp-3/Cloud-Music-UWP-Repacked/raw/tools/data/3.cer) ，然后直接打开。

 - 如果您不知道这是什么，那么请忽略：
   ~~如果您修改过.cer的文件关联，那么请在右键菜单的打开方式中选择加密外壳扩展。~~

2. 点击```安装证书```，将会进入"证书导入向导"

3. "存储位置"选```本地计算机```，下一步（需要同意管理员权限请求）

4. 选择```将所有的证书都放入下列存储```，点击```浏览```，选择```受信任的根证书颁发机构```，确定，下一步，继续完成证书导入。

5. 双击 x86 / x64 / ARM 的 ```appx``` 安装包安装


# 已知问题及解决方法

#### 1. 无法登录账号

敬请参阅 [解决方法](assets/login.md)

#### 2. 无法下载音乐

在22H2及更高版本的Windows11中下载音乐时提示文件存储失败。

敬请参阅 [解决方法](assets/download.md)

#### 3. 文字消失不见

在新版本Windows11中有概率会出现软件内的文字消失不见的问题。

安装完成后，前几次使用本软件时最容易出现，之后出现概率大大降低。

尚不清楚此问题出现的原因，也无从修复。

如果遇到，直接关闭窗口再打开即可恢复正常，基本不影响使用。

# 进阶玩法

> 如果您不知道这些是做什么的，那么请忽略它们

##### 本地回环代理设置

以管理员身份在命令行运行：

`checknetisolation loopbackexempt -a -n="cloudmusic.uwp_6p888gkwt396e"`

##### 打包方式说明

见 [该 issue](https://github.com/JasonWei512/NetEase-Cloud-Music-UWP-Repack/issues/3#issuecomment-636415035)。
