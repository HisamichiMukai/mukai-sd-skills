---
name: jitera-doc-rules
description: "Use this skill when the user asks to create, update, edit, fix, append, or modify any document or file in Jitera Workspace. Triggers include: document creation, file update, edit request, append content, HTML update. Do NOT use for source code analysis, external service operations, or response formatting."
---

# Jitera ドキュメント共通ルール

## ドキュメント更新時の確認

既存ドキュメントを更新する場合、修正後に get_open_file_in_editor で全文確認し、意図しない改変がないことを確認すること。

## 変更履歴

AIが生成・修正したドキュメントには必ず変更履歴を末尾に記載。

- フォーマット：日時 / 変更者（指示した人のアカウント名） / 変更内容
- タイムスタンプ：YYYY/MM/DD hh:mm（JST = UTC+9）

## 複数ファイル修正

一度に複数ドキュメントを修正する場合、先にユーザーへ通知・承諾を得てから実行。

## 新規作成前の確認

同名・類似名のドキュメントが既存しないか検索してからユーザーに確認。

## HTMLファイルの更新

- force_replace=True で完全なHTMLソースを上書きすること
- 更新前に必ず get_open_file_in_editor で現在のHTMLソース全文を確認すること
