---
name: create-pull-request
description: Use when the user wants a Pull Request for the changes on the current branch — e.g. "この変更の PR を作って", "create a pull request".
---

このブランチでおこなった変更について GitHub に Pull Request の Draft を作成してください。

- Title には Prefix をつける。(feat/fix/update/refactor/test/chore など)
  - refactor は、機能や挙動に一切変更がない場合のみ使用する
  - chore は、プロダクトに関係ない変更の場合のみ使用する
  - 判断できない場合は AskUserQuestion ツールで確認して
- Description のフォーマットは .github/PULL_REQUEST_TEMPLATE.md ファイルをベースにする
- Description をファイルに一時保存する場合、プロジェクト配下に .pr-{number}-{summary}.md というファイル名を作成する
- 文章は敬体「です・ます調」でなく、常体「だ・である調」で記述する。
- 文章は自動で折り返して表示されるため、一定の文字数で意図的に改行を含めたりしない。
- 具体的なソースコードについてどこをどう直したか(Where/What)の詳細は記述せず、修正方針やその理由(How/Why)について記述する。
- Title/Description の内容は確認させて。承認後に Pull Request を作成すること。
- Assignee は @yoshiharu-hirose とする。
- Labels に「機能改善」「不具合修正」のいずれかを設定する。(存在しない場合は除く)

作成が完了したら Pull Request の URL を教えてください。
