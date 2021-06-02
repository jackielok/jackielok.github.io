---
layout: post
title: "Hello World!"
date: 2020-12-29 23:00:00 +1100
categories: test maths
tags: LaTeX apples bananas
---

Hello World!

---

**Euler's formula:** For a complex number $z \in \mathbb{C}$, we can express it in polar form as $z = r e^{i \theta}$, where

$$
e^{i\theta} = \cos(i\theta) + i \sin(i\theta) , \quad \theta \in \mathbb{R} .
$$

---

&nbsp;

(We just added a blank line by `&nbsp;`.)

This is an inline formula: $y = ax^2 + b$.

We can even do multi-line equations:

$$
\begin{align}
(a+b)^2
	&= (a+b)(a+b) \\
	&= a^2 + 2ab + b^2 .
\end{align}
$$

Pretty neat! For displayed equations, a blank line needs to be left even if `$$ ... $$`` is used:
$$
y = mx + b
$$

What about matrices? (Note that the LaTeX `\\` new line might need to be doubled depending on the content-management systems -- we are passing through many layers! For example, what we have here works with `\\` as per usual. However, to escape the dollar sign `\$` not within the LaTeX environment, we actually need to write `\\$`!  

$$
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
$$

We can also do boxed environments (e.g. for theorems) by combining the LaTeX + MathJax syntax (i.e. `$ $` and `$$ $$` (plus spaces!) delimiters for inline/display maths)  with the HTML element `<div>` and the CSS style `.Boxed` that we have added in.

<div class="Boxed">
<b>Theorem 1:</b>
Let $D(z_0, r)$ be a disk in the complex plane, and $f : D(z_0, r) \to \mathbb{C}$ be a polynomial of degree $n \geq 1$ with $f'(z) \ne 0 $ for all $ z \in D(z_0, r)$. Then $f$ is injective on $D(z_0, \sin \frac{\pi}{n})$.
</div>

So we can rewrite Euler's formula from above in a much nicer way:

<div class="Boxed">
<b>Euler's formula:</b>
For a complex number $z \in \mathbb{C}$, we can express it in polar form as $z = r e^{i \theta}$, where

$$
e^{i\theta} = \cos(i\theta) + i \sin(i\theta) , \quad \theta \in \mathbb{R} .
$$
</div>

Nice! We just have to be careful if we want to say \\$10, \\$50, \\$100 instead (have to escape dollars now, and escape it doubly so with `\\`, since we are passing through two parsers!)

<div class="Boxed">
A story we tell with apples.
<br>
Then we break again, with bananas.
</div>

Cool beans, indeed.