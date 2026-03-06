# Button Component の使い方

このドキュメントでは、提供されている `Button Component` の使用方法について説明します。

## 概要

`Button Component` は、ユーザーのアクションを促すための基本的なボタン要素です。赤い背景に白いテキストが特徴で、ホバー時およびアクティブ時（クリック時）に色が変化するアニメーションが設定されています。

## HTMLの構造

ボタンを使用するには、以下のHTMLを配置します。

```html
<button class="sample-button">サンプルボタン</button>
```

※ リンク（`<a>`タグ）として使用したい場合は、クラスをそのまま適用して以下のように記述することも可能です。

```html
<a href="#" class="sample-button" style="display: inline-block; text-decoration: none;">リンクボタン</a>
```

## 必要なCSSスタイル

ボタンの見た目を適用するには、以下のCSSクラス `.sample-button` をスタイルシート（または `<style>` タグ内）に追加してください。

```css
.sample-button {
  /* サイズとフォント設定 */
  padding: 12px 24px;
  font-size: 16px;
  font-weight: bold;
  
  /* 色の設定 */
  color: #ffffff;
  background-color: #bf0000;
  
  /* 枠線と角丸の設定 */
  border: none;
  border-radius: 4px;
  
  /* マウスカーソルとアニメーションの設定 */
  cursor: pointer;
  transition: background-color 0.2s ease;
}

/* マウスオーバー時（ホバー）のスタイル */
.sample-button:hover {
  background-color: #990000;
}

/* クリック時（アクティブ）のスタイル */
.sample-button:active {
  background-color: #800000;
}
```

## クラスの詳細説明

- `.sample-button`: ボタンの基本となるスタイルです。背景色は `#bf0000`（赤系）、文字色は白になります。角丸（`border-radius: 4px`）がついており、少し柔らかな印象を与えます。
- `.sample-button:hover`: マウスカーソルがボタンに乗ったときのスタイルです。背景色が少し暗い赤（`#990000`）に変化し、クリックできることをユーザーに視覚的に伝えます。
- `.sample-button:active`: ボタンをクリック（長押し）している瞬間のスタイルです。さらに暗い赤（`#800000`）に変化し、押し込んだ感覚を表現します。
