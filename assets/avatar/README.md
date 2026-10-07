# 表情集アバター（SVG）

お手持ちのイラストをもとに、顔の輪郭・髪・服はなぞって取り出し、目・眉・口・手は描き起こしたSVGです。画像は使っていません。

| ファイル | 内容 |
|---|---|
| `expression-sheet.svg` | 9つの表情を3×3に並べた一覧 |
| `expression-<名前>.svg` | 表情ごとの単体SVG（smile, surprised, thinking, laugh, calm, shy, excited, sleepy, worried） |
| `avatar-css-switch.svg` | 9表情を1つに入れたSVG。ルート要素の `data-expr="smile"` などを書き換えるだけで、CSSで表情が切り替わる |

## CSSで切り替える使い方
`avatar-css-switch.svg` を HTML に貼り込み、`data-expr` に次のいずれかを指定します。

`smile` `surprised` `thinking` `laugh` `calm` `shy` `excited` `sleepy` `worried`

```js
document.querySelector('.avatar').setAttribute('data-expr', 'laugh');
```
