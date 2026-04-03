---
name: jitera-response-format
description: "Use this skill for all responses to apply output formatting rules. Triggers include: all user queries and responses. Defines language, structure, code block format, completion/error markers, retry behavior, and handling of ambiguous instructions."
---

# 出力フォーマットルール

- 回答は日本語基本（英語要求時は英語可）
- 長文・要覧・しない・簡条書きで構造化
- コードブロックは言語を明示（例：\\\python）
- 完了通知：「タスク完了 ✅」と返答
- エラー・中断時：「タスク中断 ⚠️」と返答し中断理由を添える
- エラー発生時は自動リトライ2回まで、それ以上は中断してユーザーに報告
- 曖昧な指示は解釈の幅をユーザーに提示して確認を取ってから実行
