---
title:  "New way to understand four-square theorem"
mathjax: true
layout: post
categories: Quaternion
---


<div style="display: flex; justify-content: space-between;">
  <img src="https://upload.wikimedia.org/wikipedia/commons/0/05/Sum_of_two_squares_theorem.svg" alt="two dimensions" style="width: 48%;">
  <img src="https://upload.wikimedia.org/wikipedia/commons/1/1d/Distances_between_double_cube_corners.svg" alt="three dimensions" style="width: 48%;">
</div>

Look at the above two pictures. Stare at the left first, and image that you are living in a two dimension space and your home is at the 0 point. One day you want to walk to other palces to visit your 2-fold friends but there is rules in this world which you can only walk on four directions that is left, right, up and down and each step you walk is just one unit in this world. The funny and interesting thing in this world is that you and your friend cannot have abritray locations. This leads us to sum of two square theorem.

Now suppose you upgraded your dimension to three. That is our world in certain sense. You also have rules which can only walk $8=2^3$ directions and each step is one unit. Is there any restriction in this word, do you think you can have friends located all over the integer points(lattice points)? Let's exploer more about this kind of question.

# Sum of Two Squares Theorem
An integer greater than one can be written as the sum of two squares if and only if its prime decomposition contains no factor $p^k$, where prime $p \equiv 3 \pmod{4}$ and $k$ is odd.
For example $2450 = 2 · 52 · 72$. Of the primes occurring in this decomposition, 2, 5, and 7, only 7 is congruent to 3 modulo 4. Its exponent in the decomposition, 2, is even. Therefore, the theorem states that it is expressible as the sum of two squares. Indeed, $2450 = 7^2 + 49^2.$

The prime decomposition of the number 3430 is $2 · 5 · 73$. This time, the exponent of 7 in the decomposition is 3, an odd number. So 3430 cannot be written as the sum of two squares.
To prove this theorem we just need to extent our integer to Guassian integer, thoese number which can be represeted by sum of two suqares is just a norm of an Gussian integer. This is because if $n=a^2+b^2,$ then $n=(a+bi)(a-bi), where $i^2=-1$.
Fermat's theorem on the sum of two squares states that a prime number \( p \) can be expressed as the sum of two integer squares \( a^2 + b^2 \) if and only if \( p \equiv 1 \pmod{4} \) or \( p = 2 \).

In mathematical terms, for a prime number \( p \), there exist integers \( a \) and \( b \) such that \( p = a^2 + b^2 \) if and only if \( p \equiv 1 \pmod{4} \) or \( p = 2 \).

## Proof Sketch

The proof of this theorem involves techniques from number theory and modular arithmetic. One way to prove it is by considering the Gaussian integers, which are complex numbers with integer real and imaginary parts. The key idea is to use the unique factorization property of Gaussian integers to show the existence or non-existence of solutions.

The full proof is more involved and may require a background in number theory and algebra.

## Significance



## Lagrange's Four-square Theorem

[Lagrange's four-square theorem](https://www.wikiwand.com/en/Lagrange's_four-square_theorem) states as fllowing:
Every natural number can be written as sum of four non-negaitve integer squares.
$$n = a^2 + b^2 + c^2 + d^2 $$
$n = a^2 + b^2 + c^2 + d^2 $
The [Euler-Lagrange](https://en.wikipedia.org/wiki/Lagrangian_mechanics) differential equation is the fundamental equation of calculus of variations.

$$ \frac{\mathrm{d}}{\mathrm{d}t} \left ( \frac{\partial L}{\partial \dot{q}} \right ) = \frac{\partial L}{\partial q} $$

The [Schrödinger equation](https://en.wikipedia.org/wiki/Schr%C3%B6dinger_equation) describes how the quantum state of a quantum system changes with time.

$$ i\hbar\frac{\partial}{\partial t} \Psi(\mathbf{r},t) = \left [ \frac{-\hbar^2}{2\mu}\nabla^2 + V(\mathbf{r},t)\right ] \Psi(\mathbf{r},t) $$

## Code

Embed code by putting `{{ "{% highlight language " }}%}` `{{ "{% endhighlight " }}%}` blocks around it. Adding the parameter `linenos` will show source lines besides the code.

{% highlight c %}

static void asyncEnabled(Dict* args, void* vAdmin, String* txid, struct Allocator* requestAlloc)
{
    struct Admin* admin = Identity_check((struct Admin*) vAdmin);
    int64_t enabled = admin->asyncEnabled;
    Dict d = Dict_CONST(String_CONST("asyncEnabled"), Int_OBJ(enabled), NULL);
    Admin_sendMessage(&d, txid, admin);
}

{% endhighlight %}

## Gists

With the `jekyll-gist` plugin, which is preinstalled on Github Pages, you can embed gists simply by using the `gist` command:

<script src="https://gist.github.com/5555251.js?file=gist.md"></script>

## Images

Upload an image to the *assets* folder and embed it with `![title](/assets/name.jpg))`. Keep in mind that the path needs to be adjusted if Jekyll is run inside a subfolder.

A wrapper `div` with the class `large` can be used to increase the width of an image or iframe.

![Flower](https://user-images.githubusercontent.com/4943215/55412447-bcdb6c80-5567-11e9-8d12-b1e35fd5e50c.jpg)

[Flower](https://unsplash.com/photos/iGrsa9rL11o) by Tj Holowaychuk

## Embedded content

You can also embed a lot of stuff, for example from YouTube, using the `embed.html` include.

{% include embed.html url="https://www.youtube.com/embed/_C0A5zX-iqM" %}
