# 基于 InterNote 的博客仓库

> 文章以 GitHub Issue 形式撰写，保存即构建，构建即上线。
>
> 本仓库由 [InterNoteTemplate](https://github.com/interset-wq/InterNoteTemplate) 模板创建，由 [Internote](https://github.com/interset-wq/InterNote) 生成器驱动。

## 快速开始

1. **创建仓库** — 点击本仓库的 **Use this template**，建议命名 `XXX.github.io`（`XXX` 为你的 GitHub 用户名）。
2. **配置站点** — 编辑 `config.toml`：站点标题、头像、giscus 评论等。键说明见 [config.sample.toml](https://github.com/interset-wq/InterNote/blob/main/config.sample.toml)。
3. **开启 Pages** — `Settings → Pages → Build and deployment → Source` 选择 `GitHub Actions`。
4. **首次构建** — `Actions → build Internote → Run workflow`，完成首次全局生成。
5. **发布第一篇文章** — 新建 Issue 并添加至少一个 Label，保存后自动构建，稍后即可通过 Pages 地址访问。

## 约定

- **文章 = Issue** — 保存/关闭 Issue 即自动构建或下线该篇；Label 用于分类。
- **生成产物必须提交** — `dist/`、`sources/`、`internote.json` 由 workflow 自动提交回本仓库，**请勿在 `.gitignore` 中忽略**。
- **首次构建后本 README 会被自动替换** 为站点统计（文章数 / 字数 / 构建时间），属正常行为。
- **修改 `config.toml` 后** 手动 `Run workflow` 全局重建一次。

## 更多

- 生成器仓库：[Internote](https://github.com/interset-wq/InterNote)
- 参考实现：[interset-wq.github.io](https://interset-wq.github.io)
