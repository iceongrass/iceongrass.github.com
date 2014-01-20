---
layout: post
title: "brew cask，Mac党的福音"
date: 2014-01-20 23:00
comments: true
categories: MacTools
---
在用惯了ubuntu上的app-get来搞软件的便捷之后，就连Windows也有了360和QQ管家之类能帮助一键安装软件的工具。在被app-store的繁琐和不给力搞到七荤八素之后，我一直都想找一个Mac上类似的工具，可诸如easy_install， pip， curl都不尽如人意。

终于，Mac党的福音来了！这就是brew cask（当当~当当当~~）

安装巨简单，两条命令搞定（前提是你已经安装了Xcode，当然你要是没装，那就忽略了这篇文章吧，下面的内容真不适合您）：

```bash
ruby -e "$(curl -fsSL https://raw.github.com/Homebrew/homebrew/go/install)
brew tap phinze/homebrew-cask && brew install brew-cask
```

<!--more-->
用法更是高大上到不需要动任何脑子：
```bash
brew cask install qq    # 安 
brew cask uninstall qq  # 卸
brew cask info qq       # 帮
brew cask search        # 查（看看都有啥可以装的，支持的软件还是蛮多的）
brew cask search qq     # 查与qq相关的软件
brew update && brew upgrade # 更新所有应用程序
```

需要注意的是，与app-store不同，通过brew cask安装的程序并没有放在`/Applications`下，而是放在`/opt/homebrew-cask/Caskroom/`，只是会在Launchpad放入快捷方式而已。

此外，brew cask上软件的更新速度会比app-store的快一些。对于一些付费的软件，brew cask默认会安装适用版。

如此简单我也就不过多啰嗦! Enjoy yourself, please~