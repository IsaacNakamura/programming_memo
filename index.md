## このページの説明

このページはPython,SQL,R,SASなどのプログラミングの技術メモです。

以下のURLでサイトにアクセスをすることができます。
https://isaacnakamura.github.io/programming_memo/

## 追記 2019/06/06

レポジトリの作り方は以下のページが参考になった。
Githubに新規リポジトリを追加
https://qiita.com/sodaihirai/items/caf8d39d314fa53db4db

## 追記 2019/06/05

プロジェクトサイトと、ユーザーサイトの作り方がそれぞれに少し変わった様子。以下参照。
https://techacademy.jp/magazine/6445


## 参照URL
Getting Started with GitHub Pages
https://guides.github.com/features/pages/

GitHub Pagesで静的サイトを簡単に作る
https://qiita.com/ririli/items/0e06b21cb709beae4514

Githubに新規リポジトリ(Repository)を作成する
https://qiita.com/bakainubau/items/4613dda50a5fa302d212

GitHubにあるリポジトリをローカルにcloneする方法
https://qiita.com/masamitsu-konya/items/abb572337156e4d003cf　　

今回はこの記事を参照してリポジトリーを作成後、ローカルにクローンする。

## サイトテンプレート

テンプレートは以下のサイト
http://www.templatewire.com/verum-free-resume-cv-template

で様々選ぶことができます。

例えば
http://www.templatewire.com/verum-free-resume-cv-template

今回はJSやphpの練習もしたいので、まずは０から書こうと思います。

## プログラミングメモ

WordPressの投稿記事内でJavascript プログラムを実行する方法
https://www.webantena.net/wordpress/run-the-javascript-in-the-article/

【CSS】おしゃれなボックスデザイン（囲み枠）のサンプル30
https://saruwakakun.com/html-css/reference/box

静的HTMLのためのテンプレートエンジン 第1回 共通部分が多いHTML
https://app.codegrid.net/entry/template-for-coding-1
--> JSを利用してやってみる。まずはとりあえず１ページづつ書く。 


## トラブルシューティング

```markdown
Permission denied (publickey).
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
```

以下のStack overflow ページを参照

Permission denied (publickey) fatal: Could not read from remote repository. while cloning Git repository
https://stackoverflow.com/questions/21255438/permission-denied-publickey-fatal-could-not-read-from-remote-repository-whil

上記サイトにより解決
```markdown
git clone git@github.com:%REPOSITORYFOLDER%/%REPOSITORYNAME%.git
```
上記は間違い。
```markdown
git clone https://github.com/%REPOSITORYFOLDER%/%REPOSITORYNAME%.git
```
こちらが正解。

次に、レポジトリにpushしようとすると、以下のエラーメッセージ
```markdown
Updates were rejected because the tip of your current branch is behind
```
[こちらのページ](https://stackoverflow.com/questions/39399804/updates-were-rejected-because-the-tip-of-your-current-branch-is-behind/39414252)を参照して解決。

```markdown
git pull origin master
git push origin master
```

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/IsaacNakamura/programming_memo/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
