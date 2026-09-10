---
name: create-issue-description
description: Use when the user wants an Issue Title and Description generated for the changes on the current branch — e.g. "この変更の issue を作って", "create an issue description".
---

このブランチでおこなった変更に対する Issue を作成する場合の Title, Description を issue-description.md ファイルに出力してください。

- Title は先頭行に h1 で記述する。
- Description のフォーマットは .github/ISSUE_TEMPLATE/ 配下の md ファイルをベースにする。複数ある場合は AskUserQuestion ツールで確認して。
- 問題の概要や修正の目的を簡潔に記述する。
