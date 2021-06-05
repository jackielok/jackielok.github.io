---
layout: post
title: "Hello World!"
date: 2021-06-01 15:00:00 +1000
categories: [development, maths]
tags: [jekyll, LaTeX]
---

Hello World! This blog allows posts to be written using [Markdown](https://www.markdownguide.org/) (for which this [Markdown cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) is very useful) and HTML/CSS, with support for maths typesetting using LaTeX + MathJax. For example, here is an inline formula formula: $y = ax^2 + bx + c$. We can also present displayed equations in their own (Markdown) section:

---

**Euler's formula:**
A complex number $z \in \mathbb{C}$ can be expressed in polar form as $z = r e^{i \theta}$, where

$$
    e^{i\theta} = \cos(i\theta) + i \sin(i\theta) , \quad \theta \in \mathbb{R} .
$$

---

&nbsp;

(We just added a blank line by using `&nbsp;`, an HTML entity.)

We can even do multi-line equations with the familiar LaTeX environments:

$$
    \begin{align}
    (a+b)^2
        &= (a+b)(a+b) \\
        &= a^2 + 2ab + b^2 .
    \end{align}
$$

Pretty neat! Note that the symbol to be used to for LaTeX commands is `$$ ... $$` (or `$ ... $` for inline formulas). Furthermore, a blank line needs to be left if a displayed formula is intended.

Note that with LaTeX support, some special characters have to be escaped (within the LaTeX environment, and also sometimes when writing normal text!) For example, a \$5 meal has to be written `a \$5 meal`, since `$` is the special character for inline LaTex `$ ... $`. As an additional note, the escaping character `\` might have to be doubled (e.g. `\\` is the special new line expression in LaTeX) depending on the content-management systems -- we are passing through many layers of parsers! So if something breaks or does not seem to work as intended, this might be the reason.

Back to the features: we can also do matrices!

$$
    \begin{pmatrix}
    1 & 0 \\
    0 & 1 \\
    \end{pmatrix}
$$

We can also do boxed environments (e.g. for theorems) by using the HTML element `<div>` and the custom CSS style `.Boxed` that we have defined, which simply adds a border (with padding, margin , etc.) to the text it surrounds. Note that this approach is very flexible and allows for much more customisation of the final appearance, but requires a fair bit more expertise in HTML/CSS development. For example:

<div class="Boxed">
<b>Theorem 1:</b>
Let $D(z_0, r)$ be a disk in the complex plane, and $f : D(z_0, r) \to \mathbb{C}$ be a polynomial of degree $n \geq 1$ with $f'(z) \ne 0 $ for all $ z \in D(z_0, r)$. Then $f$ is injective on $D(z_0, \sin \frac{\pi}{n})$.
</div>

(This was taken from <https://terrytao.wordpress.com/2020/11/28/holomorphic-images-of-disks/> just for illustration!)

Thus, we can rewrite Euler's formula from above in an alternative, seemingly nicer way:

<div class="Boxed">
<b>Euler's formula:</b>
A complex number $z \in \mathbb{C}$ can be expressed in polar form as $z = r e^{i \theta}$, where

$$
e^{i\theta} = \cos(i\theta) + i \sin(i\theta) , \quad \theta \in \mathbb{R} .
$$
</div>

Nice! We just have to be careful if we want to say \\$10, \\$50, \\$100 instead (have to escape dollars now, and escape it doubly so with `\\`, since we are passing through two parsers!)

An example that the HTML element `<br>` can produce line breaks:

<div class="Boxed">
Shopping for apples, and then,
<br>
after a break, for bananas.
</div>

<!-- 
Example of quick implementation of CSS styles for one-time use (we have implemented these in "_sass/custom.scss" instead)
<style>
  .TextWrapRight {
  display: block;
  margin: 10px;
  clear: both;
  float: right;
}
</style>
-->

<figure class="TextWrapRight" style="width:25%">
<a href="{{ site.baseurl }}/assets/images/duck.jpg">
    <img src="{{ site.baseurl }}/assets/images/duck_thumbnail.jpg" alt="A picture of a duck" style="width:100%"/>
</a>
<figcaption style="text-align: center"><i>A picture of a duck</i></figcaption>
</figure>

Another cool thing is that images and pictures can also be included, using HTML and CSS. For example, this `<img>` of a duck has been right-aligned by using a custom CSS style `.TextWrapRight` inside an HTML `<figure> ... </figure>` element.


