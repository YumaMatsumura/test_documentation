# test_documentation
## 環境セットアップ
```bash
pip3 install mkdocs
```
```bash
pip3 install mkdocs-material
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

## mkdocs.ymlの編集
```
site_name: [ドキュメント名]
nav:
  - [ページ名]: [ファイル名].md
thema: [テーマ名]
```

## 参考
- https://blog.goediy.com/?p=502

