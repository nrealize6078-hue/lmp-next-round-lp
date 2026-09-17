# LMP LP｜この街で、まだ終われない。

賃貸仲介・管理会社向け LIFE MAKE PARTNERS 加盟訴求LP（ボクシング版 / THE NEXT ROUND IS YOURS.）

検索エンジンには掲載しません（noindex）。

## ファイル

| ファイル | 中身 |
|---|---|
| `index.html` | 本文（見出し・文章・FAQ） |
| `style.css` | 前半＝土台のデザイン／後半「Boxing campaign」＝黒赤配色の上書き／末尾＝LINE相談カードと固定ボトムバー |
| `script.js` | LINEボタンの画像フォールバック、固定バーのせり上がり |
| `boxing-hero.jpg` | ヒーロー画像（1536×1024） |
| `robots.txt` | 検索非掲載 |

## 編集のしかた

- **文章を直す** → `index.html`
- **色を変える** → `style.css` 後半の先頭
  `--ink:#141414`（黒） `--blue:#bd2927`（赤） `--lime:#f1d6a7`（ベージュ） `--paper:#efede8`（背景）
- **LINEのリンク先** → `index.html` 内の `https://lin.ee/vV1leDB` を置換（2か所＋ヘッダーナビ1か所）

`hidden` 属性は CSS の `display` に負けるため、`style.css` の `[hidden]{display:none!important}` は消さないこと（消すとLINEボタンが二重に出る）。

## ローカル確認

```
python -m http.server 8970
```

## 公開

`main` ブランチに push すると GitHub Pages に反映されます。
