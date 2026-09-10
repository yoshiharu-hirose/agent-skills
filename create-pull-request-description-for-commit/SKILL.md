---
name: create-pull-request-description-for-commit
description: Use when the user wants a Pull Request description generated for a specific commit — e.g. "コミット XXX の PR description を作って", "create PR description for commit". The commit hash/ref is supplied by the user.
---

コミット $ARGUMENTS でおこなった変更を Pull Request するための Description を commit-$ARGUMENTS-description.md ファイルに出力してください。（$ARGUMENTS はユーザーが指定するコミットの識別子）

- Title には Prefix をつける。(feat/fix/update/refactor/test/chore など)
  - refactor は、機能や挙動に一切変更がない場合のみ使用する
  - chore は、プロダクトに関係ない変更の場合のみ使用する
  - 判断できない場合は AskUserQuestion ツールで確認して
- Description のフォーマットは .github/PULL_REQUEST_TEMPLATE.md ファイルをベースにする
- 文章は敬体「です・ます調」でなく、常体「だ・である調」で記述する。
- 文章は自動で折り返して表示されるため、一定の文字数で意図的に改行を含めたりしない。
- 具体的なソースコードについてどこをどう直したか(Where/What)の詳細は記述せず、修正方針やその理由(How/Why)について記述する。
