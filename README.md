# Windows-Terminal

最终还是选择了 Windows Terminal，以下为个人配置，仅供参考

## 基础搭配

- 主题：Dracula

- 字体：Fair Code

## 效果图

话不多说，先上效果图，每个人的审美都有所不同，自己感觉还不错就好。

- PowerShell

![](https://ae01.alicdn.com/kf/H7b23a9c3590d4327be7da4e89c6dc042i.jpg)

- Ubuntu

![](https://ae01.alicdn.com/kf/Hb701d26a789c4b2ea94139f7df7dd21c3.jpg)

至于为什么不用透明度，是因为真的不喜欢切换的时候各种变化，尤其是特别明显的变化。有需要可自行调整。

## 使用说明

关于 Windows 下的 bash 安装，再次就不做说明，有需要请自行查阅，一是讲解的文章很多，二是他并不是这里要说的重点。


打开 Windows Terminal 的 `Settings`选项，并将`Microsoft.PowerShell_profile`内的内容复制到你的设置中保存即可。

### 安装 oh-my-posh

运行命令以安装 posh-git

```bash
bashInstall-Module posh-git -Scope CurrentUser
```

当然可能会询问是否安装 `NuGet`，选择是，也可能会询问是否执行`Set-ExecutionPolicy`，这里选择全是，等一切安装之后，再运行以下命令安装 oh-my-posh 本身。

```bash
Install-Module oh-my-posh -Scope CurrentUser
```

### 启用模组并设置主题

启用安装的模组,运行以下命令：

```bash
Import-Module oh-my-posh
```

需要让 PowerShell 每次启动的时候都能够加载这个模组，所以我们需要设置`profile `文件让它自动启用，输入以下命令会告诉你具体的文件位置。

```zsh
$profile
```

编辑文件将我的配置文件内容复制粘贴即可。


## 相关项目

[Fair Code](https://github.com/tonsky/FiraCode)

[Dracula](https://draculatheme.com/powershell/)



## 参与我们

如果有任何想法或需求，可以在 [issue](https://github.com/tickmao/Windows-Terminal/issues) 中告诉我们，欢迎各种小伙伴踊跃留言。

## Author

Windows Terminal ©[Tickmao](https://www.tickmao.com), Released under the MIT License.

Blog @[Tickmao](https://www.tickmao.com) · GitHub @[Tickmao](https://github.com/tickmao) · Twitter @[Tickmao](https://twitter.com/Tick_puppet)
