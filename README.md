# chenxi 的最简免费博客（GitHub Pages 模板）

## 使用方法（全程只需浏览器，无需安装任何软件）

1. 登录 GitHub（用户名：chenxi）
2. 新建仓库，名字必须是：`chenxi.github.io`，勾选 Public
3. 上传以下文件（网页端 Add file → Upload files，或 git push）：
   - `_config.yml` —— 站点名 `chenxi'log`、主题、导航配置
   - `index.md` —— 首页（自动列出文章摘要）
   - `posts.md` —— 「文章」页，纯标题列表
   - `archive.md` —— 「归档」页，按年份分组
   - `about.md` —— 关于页（不在导航里，可通过 <u>about</u> 访问）
   - `_posts/2026-11-23-hello-world.md` —— 示例文章
4. 等待 1~2 分钟，访问 `https://chenxi.github.io` 即可看到博客
5. 以后发文章：在 `_posts` 里新建 `YYYY-MM-DD-标题.md` 文件，保存即发布

## 导航栏

导航栏**完全由 `_config.yml` 里的 `header_pages` 决定**，顺序就是列表顺序：

```yaml
header_pages:
  - posts.md
  - archive.md
```

想增删导航项：在上面列表里加/删文件名即可（文件必须存在于仓库根目录）。  
要加回「关于」就把 `- about.md` 加进列表。

## 注意事项

- 仓库名就是你的网址，所以必须是 `chenxi.github.io`（一字不差）
- `_posts` 里的文件名**必须**以 `年-月-日-` 开头，否则不会被识别为文章
- minima 主题**没有**搜索、标签、RSS 按钮，只有极简的标题 + 导航 + 文章列表
- 想换外观：把 `_config.yml` 里的 `theme:` 换成其他 GitHub 官方主题，  
  如 `jekyll-theme-cayman`、`jekyll-theme-hacker`（无需任何构建配置）
- 网站永久免费、由 GitHub 官方托管，只要账号在就能一直用

## 如果以后想要「搜索 + 标签」

minima 做不到，需要换主题（推荐 `jekyll-theme-chirpy`，支持归档/标签/搜索）  
或迁移到 Hugo + PaperMod（就是 Lil'Log 用的那套）。Markdown 文章可以直接搬。
****
