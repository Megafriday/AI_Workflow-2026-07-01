# AI Workflow

AIと共同で業務を進めるためのワークフローです。

## Workflow

```text
PLAN
↓
SPEC
↓
TODO
↓
TASK
↓
KNOWLEDGE
```

## Documents

| File         | Purpose                    |
| ------------ | -------------------------- |
| PLAN.md      | 要件・目的を整理する       |
| SPEC.md      | 人間とAIの認識を合わせる   |
| TODO.md      | 作業計画・進捗を管理する   |
| KNOWLEDGE.md | 再利用可能な知識を蓄積する |

## Usage

作業の開始・再開時は `master-workflow` を実行します。

`master-workflow` が現在の状態を確認し、必要に応じて各 Skill を実行します。
