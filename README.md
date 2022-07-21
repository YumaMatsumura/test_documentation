# test_documentation
## 環境セットアップ
**mkdocsを利用するためのパッケージ**  
```bash
pip3 install mkdocs
```
**ja対応するために必要なパッケージ**  
```bash
pip3 install mkdocs-material
```
**数式を利用するために必要なパッケージ**  
```bash
pip3 install pymdown-extensions
```

## ドキュメントの作成手順（備忘録）
1. まず、以下のコマンドでドキュメントを新規作成する。
```bash
mkdocs new [ドキュメント名]
```

2. \[ファイル名\]のフォルダが作成されるので、そこのフォルダまで行く。
```bash
cd [ドキュメント名]
```

**フォルダ構成**  
<pre>
[ドキュメント名]
├── mkdocs.yml
└── docs：ページを増やすときは、ここにmdファイルを追加する
    └── index.md
</pre>

3. 表示のテストをしたいときは、以下のコマンドを実行し、http://127.0.0.1:8000/をブラウザで開く。
```bash
mkdocs serve
```

4. githubと連携させたいときは、一つ前のディレクトリに戻り、gh-deployを実行する。実行することで、新たにgithubにgh-pagesブランチが作成される。
```bash
cd ..
mkdocs gh-deploy
```

## mkdocs.ymlの編集
```
site_name: [ドキュメント名]
nav:
  - [ページ名]: [ファイル名].md
thema: [テーマ名]
```

## 参考
- https://blog.goediy.com/?p=502
- https://zenn.dev/mebiusbox/articles/81d977a72cee01
- https://aiedoc.github.io/note/Tips/Mkdocs/mkdocs%E3%82%92%E4%BD%BF%E3%81%A3%E3%81%9FGitHubPages/

