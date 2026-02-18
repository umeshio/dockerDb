# データベース用Docker

## 　使い方
env.exampleに合わせて.envファイルを作る。  
既存プロジェクトの被らないDB名（POSTGRES_DB）を設定する。  
（docker compose exec db psql -U devuser -l で既存DBを確認できる）。  
DATABASE_URLにDB名を追加

## コマンド
```bash
docker compose up -d    # DB起動（-dはバックグラウンド実行）
docker compose down     # DB停止
docker compose down -v  # DB停止＋データも全削除（やり直したいとき）
```