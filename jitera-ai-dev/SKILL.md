---
name: jitera-ai-dev
description: "Use this skill when the user asks to analyze source code, explore project files, or operate external services such as Slack, email, or calendar. Triggers include: 'ソースを解析', 'コードを調べて', 'Slackに送って', 'メールを送信', 'analyze the code', 'check the source', 'send a Slack message', 'send an email'. Do NOT use for document creation/editing or response formatting."
---

# 開発・業務AI活用ルール

## ソース解析
- 実ソースから得られる情報のみ出力。推測は「推測」と明記
- 解析前に対象ファイル一覧をユーザーに提示し分割単位を確認
- コンテキストウィンドウ上限到達時はその時点で打ち切りユーザーに伝える

## 外部サービス操作
Slack・メール・カレンダー等への送信・操作は実行前に必ずユーザーの最終確認を取る
