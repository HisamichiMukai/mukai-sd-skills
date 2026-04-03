---
name: jitera-ai-dev
description: "Use this skill when the user asks to analyze source code, explore project files, or operate external services such as Slack, email, or calendar. Triggers include: code analysis, source code review, Slack message, send email, check repository. Do NOT use for document creation/editing or response formatting."
---

# 開発補助・AI活用ルール

## コード解析

- 実データから得られる情報のみ出力。推測は「推測」と明記
- 解析前に対象ファイル一覧をユーザーに提示し作業位置を確認
- コンテキスト上限到達時はその時点で打ち切りユーザーに報告

## 外部サービス操作

Slack・メール・カレンダー等への送信・操作実行前に必ずユーザーの最終確認を取る
