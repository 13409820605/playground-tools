https://mp.weixin.qq.com/s/6-2npoq9toNTpcXWrFJ2RA         #WordPress游乐场工具

这个存储库包含使用[WordPress游乐场](https://developer.wordpress.org/playground/):

-   [WordPress的游乐场插件，用于克隆你的网站](。/套餐/游乐场/)
-   [古腾堡游乐场街区](。/包/WordPress-游乐场-街区/)
-   [古腾堡的交互式代码块](。/包/交互式代码块/)
-   [Visual Studio代码的WordPress游乐场](。/packages/vs code-扩展/)
-   [WP-现在](。/包/WP-现在/)

如果你正在寻找游乐场，你可以在这里找到它:[wordpress软件游乐场](https://developer.wordpress.org/playground/)

##贡献的

Playground Tools are in their early days. If the feature you need is missing, you are more than welcome to start a discussion, [open an issue](https://github.com/WordPress/playground-tools/issues), and even propose a Pull Request to implement it.

## Getting started

Clone the repo and build the projects:

```bash
git clone https://github.com/WordPress/playground-tools
cd playground-tools
npm install
npm run build
# or `npm run dev` to watch for changes
```

You'll find the built assets in the dist directory. You can make changes, run the VS Code extension or install the interactive code plugin, and test them.

## Debug Flags

The following flags are available on the `wp-now` cli tool to aid in debugging:

-   `--inspect` - Connect to a Node debugging client.
-   `--inspect-brk` - Connect to a Node debugging client, break immediately on script execution start.
-   `--trace-exit` - Prints a stack trace whenever an environment is exited proactively, i.e. invoking process.exit().
-   `--trace-uncaught` - Print stack traces for uncaught exceptions; usually, the stack trace associated with the creation of an Error is printed, whereas this makes Node.js also print the stack trace associated with throwing the value (which does not need to be an Error instance).
-   `--trace-warnings` - Print stack traces for process warnings (including deprecations).

### Usage:

```bash
npx wp-now start [FLAGS]
```

### Connecting to DevTools

When connecting to DevTools with `--inspect` or `--inspect-brk`, the NodeJS debug icon should appear in green at the top left of the DevTools window, click on it.

![image](https://github.com/WordPress/playground-tools/assets/640101/3e5d2016-2088-432b-8312-5334a639662b)

You should see the step-debugger open, with the script paused on the first line if `--inspect-brk` was selected:

![image](https://github.com/WordPress/playground-tools/assets/640101/5f3217d0-f447-44a1-9e72-c501359d9f2a)
