# nippo

日報を投稿するリポジトリ

## github の運用ルール

このプロジェクトは、`IDD(Issue Driven Develop)`で行います！

### IDD(Issue Driven Develop)とは？

issue に対する開発を行い、必ず PullRequest も issue に向けた変更になっているように設計する開発手法です。

### ルール

1. main ブランチ への直接 Push は 🆖
2. ブランチルールに則った Branch 名で作業ブランチを切ること
3. PullRequest は必ず main ブランチ に向けて作ること

### ブランチルール

```
feat/[issue番号]/[issueの内容（英語で）]

[例]
feat/1/createBaseWebApplication
```

### 作業の流れ

1. [Project](https://github.com/CATechAccel/learn-golang/projects/1)を確認して自分がアサインされている issue がないか確認
2. アサインされている issue の中から実装しようと決めた issue を「In Progress」に移動する
3. main ブランチをチェックアウトして、`git pull`する
4. ブランチルールに従い、作業用のブランチを新規作成
5. issue 内容を満たすようにローカル環境で開発を進める
   1. commit はできるだけ作業内容が後から追ったときにわかりやすい単位で細かく切ること！
   2. コミットメッセージは日本語で良いので丁寧に書くこと！
6. 開発が完了したら、`main`←`作業ブランチ`の PullRequest を作成する
7. Pull Request に`close #1`のように close コマンドを入力して、Pull Request をマージしたら紐づく issue が close されるようにしておく
8. Reviewers, Assignees, Labels の項目を issue と合わせて設定しておく
9. 「Files changed」で自分の書いたコードにバグなどがないか一通りチェックする
10. Reviewer に設定した人に Slack の`#notify-github`でレビュー依頼をする（レビュー依頼時は Pull Request のリンクも添付しましょう）
