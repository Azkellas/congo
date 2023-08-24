---
title: Notación matemática
date: 2019-03-08
description: Una breve muestra de notación matemática en Congo.
tags: ["sample", "katex", "maths", "shortcodes"]
---

Una breve muestra de notación matemática en Congo.

<!--more-->


Congo sólo incluirá los recursos de KaTeX en su proyecto si hace uso de la notación matemática. Para que esto funcione, congo proporciona dos shortcodes: [`katexblock` y `katexinline`]({{< ref path="docs/shortcodes#katex" lang="en" >}}).
Cualquier sintaxis KaTeX en esa página dentro de cualquiera de los dos shortcodes se renderizará automáticamente.

Utilice la documentación en línea de [funciones TeX admitidas](https://katex.org/docs/supported.html) para conocer la sintaxis disponible.

## Notación en línea

La notación inline puede generarse envolviendo la expresión en el shortcode `katexinline`.

**Ejemplo:**

```tex
% KaTeX notación en línea
Notación en línea: {{</* katexinline */>}}\varphi = \dfrac{1+\sqrt5}{2}= 1.6180339887…{{</* /katexinline */>}}
```

Notación en línea: {{< katexinline >}}\varphi = \dfrac{1+\sqrt5}{2}= 1.6180339887…{{< /katexinline >}}


## Notación en bloque

Alternativamente, puede generarse una notación en bloque utilizando el shortcode `katexblock`. Esto mostrará la expresión en su propio bloque HTML.

**Ejemplo:**

```tex
% KaTeX notación en bloque
{{</* katexblock */>}}
 \varphi = 1+\frac{1} {1+\frac{1} {1+\frac{1} {1+\cdots} } }
{{</* /katexblock */>}}
```

{{< katexblock >}}
 \varphi = 1+\frac{1} {1+\frac{1} {1+\frac{1} {1+\cdots} } }
{{< /katexblock >}}
