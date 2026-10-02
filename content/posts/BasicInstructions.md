+++
date = '2026-09-27T19:23:45+08:00'
draft = false
title = '一些基础指令的记录'
+++

## 记录一下常用的一些指令

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