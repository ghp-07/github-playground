# 贡献指南

感谢你想为这个项目做点事情！下面是参与流程。

## 环境准备

```powershell
git clone git@github.com:ghp-07/github-playground.git
cd github-playground
git config user.name "你的名字"
git config user.email "你的邮箱"
```

## 工作流程

1. **先同步**，避免一开工就落后
   ```powershell
   git switch main
   git pull
   ```

2. **开分支**，不要直接在 main 上改
   ```powershell
   git switch -c feature/你的改动主题
   ```
   分支命名习惯：
   - `feature/xxx` 新功能
   - `fix/xxx` 修 bug
   - `docs/xxx` 改文档

3. **小步提交**，每条提交只做一件事
   ```powershell
   git add .
   git commit -m "docs: 补充安装说明"
   ```

4. **推送分支**
   ```powershell
   git push -u origin feature/你的改动主题
   ```

5. **开 Pull Request**，在 GitHub 页面上点 `Compare & pull request`

## 提交信息规范

```
类型: 做了什么
```

| 类型 | 用途 |
|---|---|
| `feat` | 新功能 |
| `fix` | 修复问题 |
| `docs` | 只改文档 |
| `chore` | 杂项，如依赖升级 |
| `refactor` | 重构，行为不变 |

❌ 不要写：`更新`、`改了一下`、`aaa`、`fix bug`

## 提交前自查

- [ ] 没有提交 `.env`、密钥、Token
- [ ] 提交信息人话可读
- [ ] 改动聚焦，没夹带无关文件
- [ ] 本地实际验证过

## 行为准则

保持友善。批评代码，不要批评人。
