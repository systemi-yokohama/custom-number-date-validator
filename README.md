# カスタム数値／日付バリデーター

## 概要

このカスタムバリデーターは以下のような背景のもと実装されました。

- input type="number" で数値のみの入力制限やスピナー UI は利用したいが `.` や `-` といった入力途中の状態は入力エラーとして扱いたい
- input type="number" で未入力の状態は未入力の状態として入力途中の状態とは区別して扱いたい
- input type="date" で日付の入力制限やカレンダー UI は利用したいが、`2023-02-29` や `2023-11-31` といった存在しない日付はエラーとして扱いたい
- input type="date" で年だけ入力し、月や日が未入力の状態は入力エラーとして扱いたい
- input type="date" で未入力の状態は未入力の状態として入力途中の状態とは区別して扱いたい

コードの詳細と利用方法は `index.html` を見ていただければわかるかと思います。

## 動作確認済みプラットフォーム

- macOS
  - Chrome: 123.0.6312.58（Official Build） （arm64）
  - Edge: 123.0.2420.53 (公式ビルド) (arm64)
  - Firefox: 123.0 (64 ビット)
  - Safari: 17.4 (19618.1.15.11.12)