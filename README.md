# BitzLayout

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

BitzLayoutは、BitzLabsエコシステムにおける「最後の共通中間表現」である**`LayoutAST`**の型定義を提供するライブラリです。

## `LayoutAST`とは

`LayoutAST`は、文書や図の論理的な構造（セマンティクス）が、具体的な描画情報（ジオメトリ）に変換された結果を表現します。ここには「見出し」や「タスク」といった意味情報は存在せず、「座標(10,20)にこのテキストを描画せよ」「この矩形を塗りつぶせ」といった、純粋な描画プリミティブのみが含まれます。

-   **主なノード**: `Document`, `Page`, `Layer`, `Box`, `Group`, `TextSpan`, `RichText`, `Line`, `Rect`, `Circle`, `Path`, `Image`など。

## このライブラリの位置づけ

-   **入力として**: `BitzRenderers` (SVG/PDF/Canvasレンダラー) は、この`LayoutAST`を解釈して具体的なファイルや描画を行います。
-   **出力として**: `BitzDoc`, `BitzPlot`, `BitzFlow`などの各ドメインライブラリに含まれるレイアウトエンジンは、それぞれの専門ASTを解釈し、最終的にこの`LayoutAST`を生成します。

`BitzLayout`は、ドメイン固有のロジックと、出力形式固有のロジックを分離するための、極めて重要な架け橋です。

### 依存関係

-   `BitzAstCore` (基底インターフェースを共有するため)

---# BitzLayout

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

BitzLayoutは、BitzLabsエコシステムにおける「最後の共通中間表現」である**`LayoutAST`**の型定義を提供するライブラリです。

## `LayoutAST`とは

`LayoutAST`は、文書や図の論理的な構造（セマンティクス）が、具体的な描画情報（ジオメトリ）に変換された結果を表現します。ここには「見出し」や「タスク」といった意味情報は存在せず、「座標(10,20)にこのテキストを描画せよ」「この矩形を塗りつぶせ」といった、純粋な描画プリミティブのみが含まれます。

-   **主なノード**: `Document`, `Page`, `Layer`, `Box`, `Group`, `TextSpan`, `RichText`, `Line`, `Rect`, `Circle`, `Path`, `Image`など。

## このライブラリの位置づけ

-   **入力として**: `BitzRenderers` (SVG/PDF/Canvasレンダラー) は、この`LayoutAST`を解釈して具体的なファイルや描画を行います。
-   **出力として**: `BitzDoc`, `BitzPlot`, `BitzFlow`などの各ドメインライブラリに含まれるレイアウトエンジンは、それぞれの専門ASTを解釈し、最終的にこの`LayoutAST`を生成します。

`BitzLayout`は、ドメイン固有のロジックと、出力形式固有のロジックを分離するための、極めて重要な架け橋です。

### 依存関係

-   `BitzAstCore` (基底インターフェースを共有するため)

---
