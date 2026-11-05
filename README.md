# 焼肉殿 英語・繁体字ページ

- 英語：https://checkkabu-byte.github.io/yakinikutono-en/
- 繁体字：https://checkkabu-byte.github.io/yakinikutono-en/zh/

この置き場（GitHub Pages）に上げたファイルが、そのままお客さまに見えるページになる。**AIが無くても、このページはブラウザだけで直せる。**

## ファイル

| ファイル | 中身 |
|---|---|
| `index.html` | 英語のページ |
| `zh/index.html` | 繁体字のページ |
| `images/` | 写真（どちらのページも同じ写真を使う） |
| `sitemap.xml` | Googleに渡すページの一覧。**記事を足したら、ここにも英語・繁体字の2つを足す** |

英語と繁体字は**別のファイル**なので、値段や営業時間を変えたときは**両方**直す。

## 直し方（パソコン・iPadのブラウザでできる）

1. GitHubにログインして、このページ（リポジトリ）を開く
2. 直したいファイル（`index.html` または `zh/index.html`）を押す
3. 右上の鉛筆のマーク（Edit this file）を押す
4. 直したい文字を探して書き換える。探すときはファイルの中の日本語の目印を使う：
   - `<!-- ===== 看板メニュー（値段を直すときはここ） ===== -->`
   - `<!-- ===== コース（値段を直すときはここ） ===== -->`
   - `<!-- ===== メニュー一覧（値段の幅） ===== -->`
   - `<!-- ===== 行き方・営業時間（営業時間・休みの日を直すときはここ） ===== -->`
   - `<!-- ===== いちばん上の大きな写真と見出し（Googleの評価・予算もここ） ===== -->`
5. 右上の「Commit changes」を押す → もう一度「Commit changes」
6. 1〜2分でページに反映される

### 気をつけること

- **書き換えるのは文字（`¥2,380` や `17:00–23:00` など）だけ**。`<` `>` で囲まれた部分や `style="…"` には触らない
- 英語の文の中で `'`（アポストロフィ）を使うのは問題ない（このファイルにはプログラムが無い部分なので）
- 営業時間を変えたときは、ファイルの上の方にある `openingHoursSpecification`（Googleに読ませる営業時間）も同じに直す
- おかしくなったら、ファイルの「History」から前の版に戻せる

## 記事

| 記事 | 英語 | 繁体字 |
|---|---|---|
| お店のこだわり（松阪牛と飛騨牛） | `articles/our-wagyu/index.html` | `zh/articles/our-wagyu/index.html` |
| 和牛・ブランド牛・A5の意味 | `articles/wagyu-and-brand-beef/index.html` | `zh/articles/wagyu-and-brand-beef/index.html` |
| なばなの里・スパーランドのあとの夕食（季節＝イルミネーションの期間を毎年直す） | `articles/dinner-near-nabana-no-sato/index.html` | `zh/articles/dinner-near-nabana-no-sato/index.html` |
| キムチ・タレ・スープ・お米（店内の手作り） | `articles/made-in-our-kitchen/index.html` | `zh/articles/made-in-our-kitchen/index.html` |

- 記事の文章を直すときは、そのファイルの `<!-- ===== 記事の本文（文章を直すときはここ） ===== -->` の下を書き換える
- トップページの「Articles」の欄に記事のカードが並ぶ（`<!-- ===== 記事（記事を足すときは…） ===== -->` の中）。記事を足したら、カードを1つ増やす（英語・繁体字の両方）
- 記事には値段を書かない（値段が変わるたびに直す所が増えるため）。値段はトップページだけ

## 写真を替えるとき

`images/` に同じ名前で上げ直す（Add file → Upload files）。名前を変えるときは、`index.html` と `zh/index.html` の中の名前も直す。

## 元になったもの

claude.ai のキャンバス「焼肉殿 英語・繁体字ページ案」（2026/11/03）を普通のHTMLに書き出したもの。今後の正データは**このリポジトリのファイル**（キャンバスは試作として残すだけ）。
