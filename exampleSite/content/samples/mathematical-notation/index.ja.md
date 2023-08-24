---
title: 数学的表記
date: 2019-03-08
description: Congoによる数学的表記の簡単なサンプル
tags: ["sample", "katex", "maths", "shortcodes"]
---

記事中の数学的表記にKaTeXを使用することができます。

<!--more-->

Congoは、数学的記法を使用する場合にのみ、KaTeXアセットをプロジェクトにバンドルします。これを動作させるために、congoは `katexblock` と `katexinline` という2つのショートコードを提供しています。
どちらのショートコードでも、そのページのKaTeX構文は自動的にレンダリングされます。

利用可能な構文については[サポートされているTeX関数](https://katex.org/docs/supported.html)のオンラインリファレンスを参照してください。


## インライン記法

インライン記法は `katexinline` ショートコードで式をラップすることで生成できる。

**例:**

```tex
% KaTeX inline notation
インライン記法: {{</* katexinline */>}}\varphi = \dfrac{1+\sqrt5}{2}= 1.6180339887…{{</* /katexinline */>}}
```
インライン記法: {{< katexinline >}}\varphi = \dfrac{1+\sqrt5}{2}= 1.6180339887…{{< /katexinline >}}

## ブロック記法

別の方法として、`katexblock`ショートコードを使ってブロック記法を生成することもできます。これは式を独自のHTMLブロックで出力します。

**例:**

```tex
% KaTeX block notation
{{</* katexblock */>}}
 \varphi = 1+\frac{1} {1+\frac{1} {1+\frac{1} {1+\cdots} } }
{{</* /katexblock */>}}
```

{{< katexblock >}}
 \varphi = 1+\frac{1} {1+\frac{1} {1+\frac{1} {1+\cdots} } }
{{< /katexblock >}}
