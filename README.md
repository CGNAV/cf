# 瓜田

--------------
正在运行

## 本地调试

下载内容和主题：

```bash
git clone --recursive https://github.com/CGNAV/cf.git
```

启动站点：

```bash
# 开发环境
hugo server
# 生产环境
hugo server -e production
```

需要更新主题时执行：

```bash
git submodule update --remote --merge themes/FixIt
```

## 修改主题源码

通过覆盖主题文件来修改主题源码，例如要修改主题的 `root/theme/layouts/_default/baseof.html` 文件，可以将主题源文件复制到 `root/layouts/_default/baseof.html` 文件，然后进行自己的修改，这样能避免升级主题时出现冲突。

## 部署

推送到 GitHub 后，GitHub Actions 会自动部署到 GitHub Pages。
