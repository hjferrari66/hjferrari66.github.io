@def title = "Primera Prueba Julia HTML Franklin"
@def hasmath = true
@def hascode = true


# Set up

## Update title

## Update config.md file

* change author

* add site name for GitHub

## Create a table of contents (optional)

\toc

## Upload using GitHub Desktop

# Examples

## How to enter text

Acá simplemente escribo el texto en markdown  (a revisar y aprender los detalles de Markdown)

## How to render math equations

Para Ecuaciones en Latex, colocar entre dobles símbolos de pesos:

$$ \underline {\underline G}_s ({\underline r}, {\underline r'}) = \frac{i}{8 \pi ^2} \int_0^{\infty} d k_x ~~\underline {\underline f}(k_x,\rho) ~ e^{i k_{z1} (z+z')} $$ 

$$ a^2 + b^2 = c^2 $$

$$ \frac{d}{dx} \int_a^x f(t)dt = f(x) $$

$$ \bar{x} = \frac{1}{n} \Bigg(\sum_{i=1}^n x_i \Bigg) = \frac{x_1 + x_2 + \cdots + x_n}{n} $$

$$
    \begin{alignedat}{3}
        2&x + y \space- &z &= &8 \\
        -3&x -y + 2&z &= \space&-11 \\
        -2&x + y + 2&z &= &-3
    \end{alignedat}
$$

$$
    M =
        \begin{bmatrix}
            \begin{aligned}
                &2 & &1 & -&1\space \\
                \space-&3 & -&1 & &2 \\
                -&2 & &1 & &2
            \end{aligned}
        \end{bmatrix}
$$

(optional: disable numbering)

## How to insert Julia code (with outputs!)

Hello, World!

```julia:./ex11
println("Hello, World!")
```

\show{./ex11}

Basic Math

```julia:./ex12
1 + 1
```

\show{./ex12}

Create Function

```julia:./ex13
function add(x, y)
    x + y
end
```

\show{./ex13}

Call Function

```julia:./ex14
add(2, 3)
```

\show{./ex14}

Random Numbers

```julia:./ex15
rand(5, 5)
```

\show{./ex15}

## How to insert a table from a CSV file

World Population by Region by Year:

\tableinput{}{./tableinput/population_by_year.csv}

@@source
Source: Wikipedia
@@

## How to insert an image file

![beeswarm plot of population by region](/assets/rndimg.jpg)

@@source
Source: Wikipedia
@@

## How to insert a clickable thumbnail to a YouTube video

[![YT thumbnail](https://img.youtube.com/vi/QLlA8CiTx5I/0.jpg)](https://youtu.be/QLlA8CiTx5I?si=Zt0C0VFlY0cwXeEV)

## How to inject raw HTML

~~~
<iframe width="560" height="315" src="https://www.youtube.com/embed/QLlA8CiTx5I?si=BpnmlyqIcvRohMB5" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
~~~



<!-- # Franklin syntax sandbox

This page is meant as a sandbox for Franklin Syntax so that you can quickly practice or experience things.

## Sandbox

Write whatever you want here to practice Franklin Syntax:

```julia:./ex1
using LinearAlgebra, Random
Random.seed!(135)
a, b = randn(50), randn(50)
println(dot(a, b))
println(sum(ai * bi for (ai, bi) ∈ zip(a, b)))
```

\output{./ex1}

(yet another example that floating point arithmetics can be complicated).

$$ \forall x \in \R:\quad \scal{x, x} \ge 0 $$

\newcommand{\E}{\mathbb E}

Surely some people remember the ordering, but I always forget:

$$ \varphi(\E[X]) \le \E[\varphi(X)] $$

for $\varphi$ convex. -->
