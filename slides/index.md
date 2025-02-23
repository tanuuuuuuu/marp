---
marp: true
theme: tanu
header: ""
footer: "© 2025 たぬ ( [@tanuhack](https://x.com/tanuhack) )"
paginate: true
---

<!-- _paginate: skip -->

# Marp によるプレゼン資料作成ガイド
Markdown から美しいスライドを作る


---

<!-- _paginate: skip -->

# アジェンダ

<div class="leading-relaxed">

1. イントロダクション
2. セットアップと基本
3. スライドデザイン
4. 画像とメディア
5. 高度な機能
6. デプロイと共有

</div>

---

<!-- header: "1. イントロダクション" -->

# Marpとは

**Marp（ Markdown Presentation Ecosystem ）** は、プレゼン資料をマークダウンで作成するためのエコシステム。

💡 主な特徴:
- マークダウン形式でスライドを作成する
- オープンソース（ MIT ライセンス）

---

# なぜ Marp を使用するのか？

1. **シンプルな記法**: マークダウンの知識があれば簡単に始められる
2. **高い生産性**:
    - テキストエディタでプレゼン資料を作成できる
    - Git でプレゼン資料のバージョン管理できる
3. **多様な出力形式**:
   - PDF、PowerPoint、HTML 等に出力できる
   - ホスティングサービスにデプロイすれば、URL でサクッと共有できる
4. **カスタマイズ性**: CSS で自由にデザインできる
5. **将来性**: テキストベースなので、生成 AI との相性が抜群に良い

---

<!-- header: "2. セットアップと基本" -->

# Marp のセットアップガイド

Marp を使用する方法は、2 つのアプローチが存在する:

1. **VS Code 拡張機能**
    - 「Marp for VS Code」をインストール
    - 

2. **Marp CLI**
    - プロジェクトベースでの開発に適したアプローチ
    - GitHub Pages などのホスティングサービスとの連携が容易

当スライドでは、継続的なデプロイメントを視野に入れ、Marp CLI をローカルプロジェクトにインストールする方法を紹介する。

---

<!-- header: "2. セットアップと基本 / Marp CLI" -->

# Marp CLI のインストール方法

プロジェクトフォルダを作成し、そのフォルダに移動して以下のコマンドを実行する。

```bash
$ npm install --save-dev @marp-team/marp-cli
```

```console
.
├── node_modules
├── package-lock.json
└── package.json
```

---

# マークダウンファイルを作成する

`slides/index.md` というファイルを作成する。

```markdown
# Slide 1

foo

---

# Slide 2

bar
```

---

# Directives

スライドの見た目や機能を設定するための特別な指示文。

---

<!-- header: "Directives" -->

## ディレクティブの記述方法は 2 種類

1. HTML コメント形式

```console
<!-- backgroundColor: #f8f9fa -->
```

2. Front-matter 形式

```console
---
backgroudColor: #f8f9fa
---
```

---

## Directives の種類

1️⃣ グローバル設定（全体に適用）

- テーマ設定 (`theme`)
- 言語設定 (`lang`)
- スタイル設定 (`style`)

2️⃣ ローカル設定（特定スライドに適用）

- ページ番号 (`paginate`)
- ヘッダー/フッター (`header`/`footer`)
- クラス (`class`)
- 背景色・画像 (`backgroundColor`/`backgroundImage`)
- 文字色 (`color`)

---

# Kroki で Mermaid を使う

![bg 90%](https://kroki.io/mermaid/svg/eNpNzr0OgjAcBPCdp7hRB-QNNIBfgxOOpEMplTZg_6S2EhTf3cJgnH93l7t1NAjFrcOliIC0RGpGMhIMcbydcm6gZNdjQrbCieAIjXbKVxtB92T0L--kUElrqdVYh4Vs7iF_40zDnBZknNVViO3wCZ4vvi9RyJ6s06ZB5ZsH2M8OJa7h0Sy6lvyfjuFe_STBlx6Lvi9UOfc=)

---

# 参考文献

- [Marpit Markdown | Marpit](https://marpit.marp.app/)
- [【VS Code + Marp】Markdownから爆速・自由自在なデザインで、プレゼンスライドを作る | Qiita](https://qiita.com/tomo_makes/items/aafae4021986553ae1d8)
- [見せてあげよう、Marp の真髄を](https://zenn.dev/ykicchan/articles/c30efd827337c3)
- [Marp(Marpit) | Qiita](https://qiita.com/takeshisakuma/items/5a61e6eac123d28602fb)