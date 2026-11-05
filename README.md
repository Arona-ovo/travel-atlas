# ATLAS · 旅行相册

推荐 GitHub 仓库名：`travel-atlas`

这是已构建好的静态网站，无需安装依赖、无需运行构建命令。包含日本相册 74 张照片、4 段实况，以及手机布局和声音交互。

## 上传和开启访问链接

1. 在 GitHub 创建名为 `travel-atlas` 的 Public（公开）仓库。仓库描述可写：`A personal travel atlas — Japan in photos and motion.`
2. 解压网站包。把本目录中的内容放到仓库根目录。仓库打开后必须直接能看见 `index.html`，同时能看见 `japan` 文件夹。不要把 ZIP 文件、`travel-atlas-github` 外层目录上传成网站。
3. 上传完成后，打开仓库 **Settings → Pages**。
4. **Source** 选择 **Deploy from a branch**；Branch 选择 **main**，文件夹选择 **/(root)**，点击 **Save**。
5. 等待 Pages 页面显示发布成功，点击它提供的链接。一般格式是 `https://你的GitHub用户名.github.io/travel-atlas/`。这才是发给手机或朋友的浏览地址，仓库的 github.com 地址不是网站。

官方设置说明：https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## 上传方式

- 推荐使用 GitHub Desktop：克隆刚创建的仓库，复制本目录全部内容到仓库目录，Commit 后 Push。这样可以一次上传全部文件，不需要命令行。
- 网页上传也可以，但 GitHub 网页单批文件数量有限。包中另附 `网页分批上传`，分两批将各批文件夹**里面的内容**拖到仓库的 Add file → Upload files 页面，每批提交一次。两批都上传到同一个仓库根目录；不要上传“第1批”“第2批”外层目录。

## 网站结构

```
index.html             旅行总站
album-summary.js       相册统计
.nojekyll              静态网站标记
japan/
  index.html           日本相册
  photos-data-web.js    照片清单
  thumbs/              缩略图
  display/             展示照片
  motion/              实况短视频
```

本包仅包含发布所需文件；本地备份、浏览器资料、原照片、测试脚本与大体积内嵌数据不在其中。继续编辑和加照片时，保留电脑上的原项目，更新后重新复制发布文件即可。

在手机上首次开启声音需要点 Sound 或页面开声按钮。实况照片带 LIVE 标记，进入大图后点“播放实况”。
