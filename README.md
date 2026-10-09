# JackAIStudio.github.io

这个仓库只做一件事：把 `robots.txt` 和 `llms.txt` 放到域名根。

GitHub Pages 上，`robots.txt` 只认域名根 `https://jackaistudio.github.io/`，
爬虫不会去看子路径下的那份。所以想让它生效，必须有一个名字正好叫
`JackAIStudio.github.io` 的仓库 —— 就是这个。

站点的实际内容在 [jackskill](https://github.com/JackAIStudio/jackskill) 仓库，
发布在 https://jackaistudio.github.io/jackskill/ 。两个仓库各管各的，互不干扰。

## 文件

- `robots.txt` —— 显式放行 AI 爬虫。只对本域名生效，管不到 github.com。
- `llms.txt` —— 本域名的索引，详细内容指向 `jackskill/llms.txt`。
- `index.html` —— 首页。

## 注意

`robots.txt` 里的规则跟着这个仓库走，改了要 push 才会生效，GitHub Pages
重建大约 20~60 秒。`jackskill` 那边的内容更新跟这里无关。
