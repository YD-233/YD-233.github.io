# YD-233 的博客

使用 Jekyll 和 GitHub Pages 发布的 Markdown 博客。

在线地址：<https://yd-233.github.io/>

## 发布新文章

1. 在 `_posts` 目录新建文件，命名为 `YYYY-MM-DD-英文短标题.md`。
2. 在文件开头填写文章信息：

   ```yaml
   ---
   layout: post
   title: "文章标题"
   categories: 分类
   ---
   ```

3. 使用 Markdown 编写正文。
4. 提交并推送到 `main` 分支：

   ```bash
   git add .
   git commit -m "发布新文章"
   git push
   ```

GitHub Actions 会自动构建并发布，通常几分钟内生效。

## 修改博客信息

博客名称、简介和 GitHub 链接在 `_config.yml` 中修改，关于页面在 `about.md` 中修改。

## 本地预览（可选）

安装 Ruby 和 Bundler 后运行：

```bash
bundle install
bundle exec jekyll serve
```

然后访问 <http://127.0.0.1:4000>。
