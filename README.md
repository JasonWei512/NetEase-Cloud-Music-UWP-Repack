<img src="https://user-images.githubusercontent.com/26399680/47980314-0e3f1700-e102-11e8-8857-e3436ecc8beb.png" alt="logo" width="140" height="140" align="right">

#  🎼 CloudMusic-UWP-Repacked 🚀

&nbsp;
&nbsp;
## 简介

经典的 **网易云音乐UWP** 重打包版客户端，不会自动更新，且可以与官方版共存。

- 合并了100和400尺寸图形资源，并首次修复了在Win11系统下的文件访问权限问题。

> 此版本只是在原版软件的基础上进行了简单地故障修复，除此外无其他多余更改，请放心使用。
> 同时，也不包含任何盗版侵权功能，您必须登录自己的会员账号才能查看付费内容。


&nbsp;
## 下载

**下载安装包：** &nbsp;&nbsp;[X64](https://github.com/exp-3/Cloud-Music-UWP-Repacked/raw/main/cloudmusic.uwp_repack_x64.appx) &nbsp;| &nbsp;[X86](https://github.com/exp-3/Cloud-Music-UWP-Repacked/raw/main/cloudmusic.uwp_repack_x86.appx) &nbsp;| &nbsp;[ARM](https://github.com/exp-3/Cloud-Music-UWP-Repacked/raw/main/cloudmusic.uwp_repack_arm.appx)

> **不确定计算机类型？**
>1. 按下 `Win + R` 键打开“运行”对话框。
>2. 输入 `msinfo32` 并按回车键。
>3. 在“系统摘要”页面中查找“系统类型”一项，它会显示您的电脑是基于哪种架构。


&nbsp;
## 安装

由于Windows只允许安装来自**微软商店**或者**企业开发者**的appx/msix软件包，<br />
所以我们需要先安装**自签名证书**来伪装成企业开发者，才能安装第三方软件包。

请选择以下其中一种方法：

#### 方法一：

1. 下载 [配套工具包](https://github.com/exp-3/CloudMusic.UWP-Tools/archive/dbb93c60c3dd9c634484ee1610f80d17dd66c02a.zip) ，务必解压缩所有文件 (不要在压缩包内打开)

2. 打开 ```一键安装根证书.bat``` ，根据提示操作即可

3. 当显示内容包含 ```证书 "patched" 添加到存储``` 或者 ```证书 "patched" 已经在存储中``` 说明安装成功

4. 下载合适的 ```appx``` 软件包，双击打开安装

> 某些杀毒软件可能会将证书安装工具误报为病毒，您可能需要暂时关闭杀毒软件或者添加白名单才能使用。或者也可以考虑使用下面的方法二。

#### 方法二：

1. 下载 [证书文件](https://github.com/exp-3/CloudMusic.UWP-Tools/raw/main/data/3.cer) ，然后直接打开。

2. 点击 ```安装证书``` ，将会进入"证书导入向导"

3. "存储位置"选 ```本地计算机``` ，下一步（需要同意管理员权限请求）

4. 选择 ```将所有的证书都放入下列存储``` ，点击 ```浏览``` ，选择 ```受信任的根证书颁发机构``` ，确定，下一步，继续完成证书导入。

5. 下载合适的 ```appx``` 软件包，双击打开安装


&nbsp;
## 已知问题及解决方法

#### 1. 无法登录账号

请参阅 [解决方法](assets/login.md)

#### 2. 无法下载音乐

在22H2及更高版本的Windows11中下载音乐时提示文件存储失败。

请参阅 [解决方法](assets/storage.md)

#### 3. 文字消失不见

在新版本Windows11中有概率会出现软件内的文字消失不见的问题。

安装完成后，前几次使用本软件时最容易出现，之后出现概率大大降低。

尚不清楚此问题出现的原因，也无从修复。

如果遇到，直接关闭窗口再打开即可恢复正常，基本不影响使用。


&nbsp;
## 进阶玩法

> 如果您不知道这些是做什么的，那么请忽略它们

##### 本地回环代理设置

以管理员身份在命令行运行：

`checknetisolation loopbackexempt -a -n="cloudmusic.uwp_6p888gkwt396e"`

##### 打包方式说明

见 [该 issue](https://github.com/JasonWei512/NetEase-Cloud-Music-UWP-Repack/issues/3#issuecomment-636415035)。
