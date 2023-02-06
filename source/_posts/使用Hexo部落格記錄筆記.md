---
title: 使用Hexo部落格記錄筆記
date: 2023-02-06 23:23:36
tags: Hexo 指令
---

hexo init ：[folder] 新建一個網站。如果沒有設置folder，Hexo 默認在目前的文件夾建立網站。
hexo new ："文章名稱" 新建一篇文章。
hexo server ：啟動服務器。默認情況下，訪問網址為：http://localhost:4000/。
hexo generate ：生成靜態文件。可以簡寫為：hexo g
hexo deploy ：部署網站。可以簡寫為：hexo d
hexo publish ：<filename> 發表草稿。
hexo clean ：清除緩存文件( db.json) 和已生成的靜態文件( public)。
hexo list < type > ：列出網站資料。 type帶入: page, post, route, tag, category
hexo version ：顯示Hexo 版本。
相關命令出處，參考https://hexo.io/zh-cn/docs/commands

npm install hexo-generator-feed --save
RSS 套件參考出處：https://ithelp.ithome.com.tw/articles/10240120

在GitHub Pages 上部署Hexo：
1.建立名為username .github.io的儲存庫，username 是你在GitHub 上的用戶名，若之前已將Hexo 上傳至其他儲存庫，將該儲存庫重命名即可。
2.將Hexo 文件夾中的文件push 到儲存庫的默認分支，默認分支通常名為main，舊一點的儲存庫可能名為master。
參考出處：https://hexo.io/zh-cn/docs/github-pages

補充，關於還原備份到 Github 另外一個分支的 Hexo 資料
1.開新分支
2.將寫文章用的 Markdown 以及 Hexo 的設定檔儲存至另一分支

參考出處:https://ithelp.ithome.com.tw/articles/10279635
        https://www.dazhuanlan.com/imdq/topics/965923