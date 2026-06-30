---
name: task-execution
description: >
  TODOに基づき1タスクずつ実行し、
  TODOを最新状態へ維持する。
---

# Task Execution

## Rules

- TODOを唯一の進捗管理とする
- TODOには担当者を付与する
- 一度に実行するタスクは1件のみ
- HUMANタスクでは停止する

## Procedure

現在の担当者を確認する

### AIタスク

- TODOを In Progress に更新する
- タスクを実行する
- 完了へ更新する

### HUMANタスク

- 実施内容を説明する
- 人間へ引き継ぐ
- 完了報告を待つ

完了後

- TODOを更新する
- 次のタスクを決定する

エラー・新しい知見・運用変更が発生した場合 → knowledge-update を実行する

## Finish

TODO.md を更新する
