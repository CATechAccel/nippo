# 日報

日報を投稿するリポジトリ

## 日報テンプレート

日報はこちらの [template.md](./template.md) をコピペして作成してください！

## 日報運用ルール

### ルール

1. main ブランチ への直接 Push は 🆖
2. ブランチルールに則った Branch 名で作業ブランチを切ること
3. PullRequest は必ず main ブランチ に向けて作ること

### ブランチルール

```
feat/[issue番号]/[日付]

[例]
feat/1/2020_11_15
```

### 作業の流れ

1. [Project](https://github.com/CATechAccel/nippo/projects/1)にて作業した日付をタイトルとした issue を作成する
2. 作成した issue を「In Progress」に移動する
3. main ブランチをチェックアウトして、`git pull`する
4. ブランチルールに従い、作業用のブランチを新規作成
5. [template.md](./template.md)の内容をコピペして、「日付.md（例：2020_11_15.md）」ファイルを作成する
6. 作成したファイルに日報を記入し、PullRequest を作成する
7. Pull Request に`close #1`のように close コマンドを入力して、Pull Request をマージしたら紐づく issue が close されるようにしておく
8. Reviewers, Assignees, Labels の項目を issue と合わせて設定しておく
9. Slack の`#times-かねぽん`で`@here`つきでレビュー依頼をする（レビュー依頼時は Pull Request のリンクも添付しましょう）
