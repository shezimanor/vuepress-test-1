# Vuepress2 試玩

> 使用 Github Actions 自動部署

框架: Vuepress2

自動部署的配置文件: `.github/workflows/docs.yml`。

流程: 當 push 到分支 `main` 後，會自動將靜態網站 push 到分支 `gh-pages`。

[網站](https://shezimanor.github.io/vuepress-test-1/)就會被更新。

---

## ACCESS_TOKEN

先從 github profile: Settings > Developer settings > Personal access tokens > Tokens(classic) > Generate new token

該 token 把 `repo` 和 `workflow` 的權限打開。(記得複製起來，只有一次機會，之後重開都要拿新的)。

再到目標 Repo > Settings > Secrets and variables > Actions > New repository secret

把取得的 token 新增進去，`.yml` 就會吃到他了。
