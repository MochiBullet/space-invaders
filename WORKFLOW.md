# Git Workflow: PC / スマホ 相互作業ガイド

## 構成

```
PC Claude ←→ GitHub (リモート) ←→ スマホ Claude
```

## 作業の流れ

1. **作業開始時**: 最新を取得
   ```bash
   git pull origin master
   ```

2. **作業**: コード変更 → commit → push
   ```bash
   git add <ファイル>
   git commit -m "変更内容"
   git push origin master
   ```

3. **もう片方の環境で作業再開**: pull してから作業開始

## 初回セットアップ（新しい環境）

```bash
git clone https://<TOKEN>@github.com/MochiBullet/space-invaders.git
```

## 注意点

- **同時に両方で作業しない** — 同じブランチを同時に触るとコンフリクトする
- 片方で push → もう片方で pull の順番を守る
- トークンが期限切れの場合は GitHub Settings > Developer settings > Personal access tokens から再発行
