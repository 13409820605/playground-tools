![上传网页截图20241009_034159.png…]()
[国军人才招募中心源起过去 - 豆丁网(1).pdf](https://github.com/user-attachments/files/18054061/-.1.pdf)
[區公所 - 善化區-公開資訊(1).pdf](https://github.com/user-attachments/files/18054059/-.-.1.pdf)
![截图_20240930_143426](https://github.com/user-attachments/assets/8083095d-8f9f-4f65-99bf-8b87ca19b1d1)![上传屏幕截图_20240930_143426.jpg...]()
    #WordPress游乐场工具

这个存储库包含使用[wordpress软件游乐场](https://developer.wordpress.org/playground/):

-   [wordpress软件的游乐场插件,用于克隆你的网站](。/套餐/游乐场/)
-   [古腾堡游乐场街区](。/包/WordPress-游乐场-街区/)
-   [古腾堡的交互式代码块](。/包/交互式代码块/)
-   [可视化工作室代码的wordpress软件软件游乐场](。/packages/vs代码扩展/)
-   [WP-现在](。/包/WP-现在/)

如果你正在寻找游乐场，你可以在这里找到它:[wordpress软件游乐场](https://developer.wordpress.org/playground/)

##贡献的

Playground Tools are in their early days. If the feature you need is missing, you are more than welcome to start a discussion, [提出一个问题](https://github.com/WordPress/playground-tools/issues), and even propose a Pull Request to implement it.

##入门指南

克隆存储库并构建项目:

```尝试
git克隆https://github.com/WordPress/playground-tools
cd游乐场-工具
npm安装
npm运行构建
#或“npm运行开发”来观察变化
```

您将在dist目录中找到构建的资产。您可以进行更改，运行VS代码扩展或安装交互式代码插件，并测试它们。

##调试标志

上提供了以下标志`WP-现在`帮助调试的硬币指示器 （coin-levelindicator的缩写）命令行界面（Command Line Interface for batch scripting）工具：

-   `-检查`-连接到节点调试客户端。
-   `-检查-刹车`-连接到节点调试客户端，在脚本执行开始时立即中断。
-   `-跟踪-退出`-每当主动退出环境时,即调用process.exit()时,打印堆栈跟踪。
-   `-跟踪-未捕获`-打印未捕获异常的堆栈跟踪；通常，会打印与错误创建相关联的堆栈跟踪，而这使得Node.js还会打印与抛出值相关联的堆栈跟踪(不必是错误实例)。
-   `-跟踪-警告`-打印进程警告(包括弃用)的堆栈跟踪。

### Usage:

```尝试
npx wp-now start [FLAGS]
```

### Connecting to DevTools

When connecting to DevTools with `--inspect` or `--inspect-brk`, the NodeJS debug icon should appear in green at the top left of the DevTools window, click on it.

![image](https://github.com/WordPress/playground-tools/assets/640101/3e5d2016-2088-432b-8312-5334a639662b)

You should see the step-debugger open, with the script paused on the first line if `--inspect-brk` was selected:

![image](https://github.com/WordPress/playground-tools/assets/640101/5f3217d0-f447-44a1-9e72-c501359d9f2a)
