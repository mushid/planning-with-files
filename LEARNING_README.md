# 学习笔记

## Remote 配置

| Remote   | 用途              |
|----------|------------------|
| origin   | 推送个人学习内容   |
| upstream | 同步上游更新       |

## 分支说明

- **main**: 保持与 upstream 同步
- **learn**: 学习分支，存放个人笔记

## 目录结构

- `learn/` - 系统性学习文档
- `notes/` - 零散笔记
- `experiments/` - 实验代码

## 同步上游更新

```bash
git fetch upstream
git checkout main && git merge upstream/main && git push origin main
git checkout learn && git rebase main && git push --force-with-lease
```
