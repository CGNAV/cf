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

## 部署

推送到 GitHub 后，GitHub Actions 会自动部署到 GitHub Pages。
