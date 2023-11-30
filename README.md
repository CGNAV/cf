# GuaTian万事屋

--------------

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
# git本地上传github

1.git init
2.git add .
3.git status
4.git commit -m "秒速"
5.git push

git reset .  这个是撤销add .


## 修改主题源码

1.通过覆盖主题文件来修改主题源码，例如要修改主题的 `root/themes/FixIt/layouts/_default/baseof.html` 文件，可以将主题源文件复制到 `root/layouts/_default/baseof.html` 文件，然后进行自己的修改，这样能避免升级主题时出现冲突。
2. 例如：我想改主题的 layouts/_default/xxx.html 文件       我就可以在自己根目录新建一个 layouts/_default/xxx.html 
3. **原理就是：hugo会优先读取博客内的同名文件，然后再去读取主题的**   
这样就可以不用把主题的全部代码上传到自己仓库，升级的时候也不会有文件冲突！

## 部署

1. 转到 Setting => Pages => Build and deployment => Deploy from a branch => 分支选择 "gh-pages"。
2. 转到 Setting => Actions => General => Workflow permissions => 选中 "Read and write permissions"。

之后每次推送到 GitHub 后，GitHub Actions 会自动部署到 GitHub Pages。
