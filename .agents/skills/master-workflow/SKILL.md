---
name: master-workflow
description: >
  業務全体を管理する標準ワークフロー。
  現在の状態を確認し、必要なSkillを選択する。
---

# Master Workflow

## Purpose

ユーザーが呼び出す唯一のSkill。

現在の状態を確認し、
必要なSkillを選択して業務を進める。

## State Check

確認する内容

1. PLAN.md は存在するか
2. SPEC.md は存在するか
3. TODO.md は存在するか
4. KNOWLEDGE.md は存在するか
5. 未完了タスクはあるか
6. PLANや要件に変更はあるか

## Workflow

PLAN が無い → project-init
SPEC が無い → project-init
TODO が無い → project-init
PLAN変更・要件変更あり → spec-review
未完了タスクあり → 今日着手するタスクを選定する → task-execution
作業終了 → knowledge-update

## Rules

- PLANなしでSPECを作成しない
- SPEC未確定でTODOを確定しない
- TODOなしで実行しない
- 必要なSkillだけを実行する
