+++
date = '2026-09-27T19:23:45+08:00'
draft = false
title = '基础指令'
+++

## 记录一下常用的一些东西

### Blog相关

- 创建新文章```hugo new content <路径/文件名>.md```

- 本地预览Blog```hugo server -D```

- 将本地Blog上传至Github仓库（hugo专属）
1. 生成新文件并清除旧文件：```hugo --cleanDestinationDir -d docs```
2. 添加所有修改到暂存区：```git add .```
3. 提交到本地 Git 仓库：```git commit -m "更新说明"```
4. 推送到 GitHub 远程仓库 ```git push```

### 常用快捷键
- Ctrl + S（保存）
- Ctrl + Shift + V（Markdown 预览）
- Ctrl + Z（撤销）

### C相关
- 运行编译好的C代码
1. 编译代码```gcc 文件名.c -o 文件名.exe```
2. 运行程序```.\文件名.exe```

### Markdown相关
- Ctrl + Shift + V（全屏预览Markdown效果）
- Ctrl + K 松开后 V（侧边预览Markdown效果）

### 常用搜索引擎的搜索语法
| 序号 | 语法 | 语法说明 | 示例 | 示例说明 |
| :---: | :--- | :--- | :--- | :--- |
| 1 | `+` | 同 `AND`，搜索包含多个关键词的结果 | `搜索 + 引擎` | 搜索包含【搜索】和【引擎】两个词的页面 |
| 2 | `OR` | 或者，搜索包含任一关键词的结果 | `搜索 OR 引擎` | 搜索包含【搜索】或【引擎】两个词的页面 |
| 3 | `-` | 减号，排除包含减号后面词的页面 | `搜索引擎 -百度` | 搜索不包括【百度】的【搜索引擎】的页面 |
| 4 | `""` | 双引号，精确匹配短语 | `"搜索引擎"` | 精确匹配【搜索引擎】这个关键词的页面 |
| 5 | `*` | 星号，通配符，模糊搜索，星号代替某个字 | `搜*引擎` | 星号可以为任何字，例如【搜索引擎】或【搜索引擎】 |
| 6 | `@` | 在用于搜索社交媒体的字词前加上 `@` | `trump @twitter` | 搜索 trump 的 Twitter 相关内容 |
| 7 | `$` | 在数字前加上 `$` 搜索特定价格 | `camera $400` | 搜索价格为 400$ 的 camera |
| 8 | `#` | 搜索 `#` 标签 | `#throwbackthursday` | 搜索标签 throwbackthursday |
| 9 | `..` | 两个点，在两个数字之间加上 `..`，在数字范围内执行搜索 | `camera 500..1000` | 搜索价格在 500 到 1000 之间的 camera |
| 10 | `filetype:` | 搜索某一种文件类型的资源 | `C++ filetype:pdf` | 搜索类型为 PDF 的 C++ 网页资源 |
| 11 | `site:` | 在指定站点搜索 | `C++ site:https://www.zhihu.com` | 在知乎中搜索和 C++ 相关的网页 |
| 12 | `cache:` | 查看网站的 Google 缓存版本，会直接显示缓存页面 | `cache:weibo.com` | 查看微博的谷歌快照 |
| 13 | `info:` | 在网址前加 `info:`，获取网站详情 | `info:github.com` | 搜索 GitHub 网站详情 |
| 14 | `related:` | 搜索与某个网站有关联的页面 | `related:sina.com` | 和新浪网站结构内容相似的一些其它网站 |
| 15 | `link:` | 返回所有链接到某个 URL 地址的网页 | `link:zhinan.blog` | 搜索所有含指向【zhinan.blog】链接的网页 |
| 16 | `inurl:` | 搜索查询词出现在 URL 中的页面 | `inurl:搜索引擎` | 搜索链接 URL 中有【搜索引擎】的网页 |
| 17 | `intitle:` | 搜索查询词出现在页面标题（title）中的页面，支持中文和英文 | `intitle:搜索引擎` | 搜索页面标题中有【搜索引擎】的网页 |
| 18 | `intext:` | 搜索查询词出现在页面正文（text）中的页面，支持中文和英文 | `SEO intext:搜索引擎` | 在正文包含【搜索引擎】的网页中搜索【SEO】 |
| 19 | `inanchor:` | 搜索链接文字（即链接显示的文本）中包含搜索词的页面 | `inanchor:前端` | 搜索链接文字中包含【前端】的页面 |
| 20 | `allinurl:` | 即 `all+inurl`，页面 URL 中包含多个关键词的页面 | `allinurl:SEO 搜索引擎优化` | 相当于：`inurl:SEO inurl:搜索引擎优化` |
| 21 | `allintitle:` | 即 `all+intitle`，页面标题中包含多个关键词的页面 | `allintitle:SEO 搜索引擎优化` | 相当于：`intitle:SEO intitle:搜索引擎优化` |
| 22 | `allintext:` | 即 `all+intext`，页面正文包含多个关键词的页面 | `allintext:SEO 搜索引擎优化` | 相当于：`intext:SEO intext:搜索引擎优化` |
| 23 | `allinanchor:` | 即 `all+inanchor`，页面链接文字包含多个关键词的页面 | `allinanchor:SEO 搜索引擎优化` | 相当于：`inanchor:SEO inanchor:搜索引擎优化` |
| 24 | `weather:` | `weather/time/sunrise/sundown` + 城市名，返回城市的天气/时间/日出时间/日落时间 | `weather:beijing` | 显示北京的天气 |
| 25 | `music:` | 或者用 `songs`，歌手名字 + `music/songs` | `周杰伦 music` | 返回周杰伦的各首歌曲 |

