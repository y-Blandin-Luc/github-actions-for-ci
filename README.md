# Tic Tac Toe Game

Learn GitHub Actions through a fun little game.
[全てのGitHub Actionsチュートリアル](https://lab.github.com/githubtraining/devops-with-github-actions)

# GitHub Actions

[GitHub Actionsのチュートリアル](https://lab.github.com/githubtraining/github-actions:-continuous-integration)でGitHub Actions（コンパイルとテスト）を定義する。

# Prettier

GitHub Actionsの続きです。

プッシュの時にフォーマットして、自動で修正コミットして、コンパイルして、テストを実行する。

1. [チュートリアル](https://mskelton.medium.com/auto-formatting-code-using-prettier-and-github-actions-ed458f58b7df)を参照する
2. 「.prettierignore」のファイルに無視するファイルフォーマット（jsファイル以外）を定義する。
3. 「package.json」にコマンドを追加して、先ほどのテストコマンドに「_npx standard_ **--fix**」を追加する
4. 「workflows/node.js.yml」にジョブを追加する

   1.ステップ1はソースコードをフォーマットする
   
   2.ステップ2はコミットする 
   
5. リポジトリにプッシュする時に、GitHub Actionsが実行される

# Eslint 

Prettierの続きです。

プッシュの時にEslintを実行して、フォーマットして、自動で修正コミットして、コンパイルして、テストを実行する。

1. [チュートリアル](https://medium.com/javascript-scene/streamline-code-reviews-with-eslint-prettier-6fb817a6b51d)を参照する
2. 「.eslintignore」、「.eslintrc」、「.prettierrc」のファイルを追加する
3. テストを実行するために「.eslintrc」に「"jest": true」を追加する
4. 「package.json」に「"lint": "eslint --fix . && echo 'Lint complete.'"」のコマンドを追加する
5. 「workflows/node.js.yml」にフォーマットのステップの前にEslintのステップを追加する
6. GitHub Actionsを実行する時に、ログにEslintの結果が表示される。問題なし場合、「Lint complete.」のみが表示される。

[Eslint](https://eslint.org/docs/user-guide/formatters/)
[Eslint & Prettierの設定](https://github.com/prettier/eslint-config-prettier)
[PrettierとEslintの統合](https://prettier.io/docs/en/integrating-with-linters.html)
