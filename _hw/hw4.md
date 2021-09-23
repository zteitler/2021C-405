---
layout: assignment
title: Homework 4
duedate: 2021-09-29
mathjax: true
---

## Instructions

Please find and use the [LaTeX template for homework]({{ "/assets/405505-Homework-template.tex" | relative_url }}).

Use LaTeX to create a PDF. Upload your PDF to Gradescope.
If you don't have LaTeX on your computer, you can use [Overleaf](https://overleaf.com).
Don't submit the LaTeX source, just the PDF.
Email your instructor (that's me) if you have questions or need help.

Please include your name and the homework number within the document.
Some additional formatting instructions are in the
[syllabus]({{ "/syllabus" | relative_url }}).
To summarize:

+ Use a new page (`\newpage`) for each problem.
+ State which question you are answering and the actual question.
  Then, start your answer in a new paragraph.
+ Use environments such as `proof` and `theorem`
  (via `\begin{proof}...\end{proof}`).
+ Use 12pt option `\documentclass[12pt]{amsart}` and linespacing `\linespread{2.4}`.


You are encouraged to [work together on the homework](https://zteitler.github.io/2021C-405/syllabus.html#a-note-on-collaboration)!


## Problems to turn in on Gradescope


1.  Section 1.5, Exercises 2, 5, 6: Try as many as you can.
    Turn in the best/most interesting one that you are able to solve.
    (For exercise 2: There is more than one way to prove this, including ideas from
    linear algebra or other classes. For this class, please follow the outline given in the hint.)

2.  Section 2.1, Exercise 1

3.  Section 2.1, Exercise 3.
    (You have to clearly state the equations, and
    show the set given by the parametrization is equal to the set defined by the equations.
    That means: any point that is given by the parametrization will satisfy the equations,
    and any point that satisfies the equations is given by the parametrization,
    in other words there are some input values that give that point as the output.)


The next two exercises are not from the textbook.

We can use ideals to define "modulo" equivalence relations in any ring.

For these exercises let $$R$$ be any commutative ring with multiplicative identity.
For any set $$S \subseteq R$$ and for any $$x,y \in R$$,
we define $$x \equiv y \pmod{S}$$, in other words $$x$$ is congruent to $$y$$ modulo $$S$$,
if and only if $$x-y \in S$$.

**LaTeX:** Write `x \equiv y \pmod{S}` to get $$x \equiv y \pmod{S}$$.
Please use the `\pmod{...}` command to write about modular congruence.
You can avoid using this notation if you simply write `x - y \in S` ($$x-y \in S$$).

The goal of these exercises is to show that this congruence relation
has nice properties, like congruence of integers (modular arithmetic),
if and only if $$S$$ is an ideal.
This is one of the reasons why ideals are defined the way they are,
and why they are important.

{: start="4"}
4.  In this exercise you will explain how this new "modulo ideals"
    is related to "modulo an integer" that you have seen before,
    and you will prove that "modulo ideals" has nice properties.
    
    1.  First suppose $$R = \mathbb{Z}$$ and $$I = \langle m \rangle$$
        is the ideal consisting of multiples of $$m$$.
        Explain why congruence modulo the ideal $$I$$ (new definition in this homework)
        is the same thing as congruence modulo $$m$$ (definition you've seen in previous classes).
    
    For the rest of this exercise let $$R$$ be any commutative ring with multiplicative identity
    and let $$I$$ be any ideal in $$R$$.
    
    {: start="2"}
    2.  Prove that congruence modulo $$I$$ is reflexive, symmetric, and transitive.
        
        (Recall: saying that congruence modulo $$I$$ is *reflexive* means that
        for all $$x \in R$$, $$x \equiv x \pmod{I}$$.
        Saying congruence is *symmetric* means that if $$x \equiv y \pmod{I}$$,
        then $$y \equiv x \pmod{I}$$.
        Saying congruence is *transitive* means that if $$x \equiv y \pmod{I}$$
        and $$y \equiv z \pmod{I}$$, then $$x \equiv z \pmod{I}$$.)
        
    3.  Prove that if $$a \equiv b \pmod{I}$$ and $$c \equiv d \pmod{I}$$,
        then $$a+c \equiv b+d \pmod{I}$$ and $$ac \equiv bd \pmod{I}$$.
        We say that congruence modulo $$I$$ is *additive* and *multiplicative*.

5.  This exercise is to show the converse:
    the "nice" algebraic properties of modular arithmetic hold *only* for ideals.
    Our goal is to prove that if congruence modulo $$S$$ has the nice properties
    in the previous exercise,
    then $$S$$ has to be an ideal.
    
    Let $$R$$ be a commutative ring with multiplicative identity
    and let $$S$$ be a subset in $$R$$.
    
    1.  Show: If congruence modulo $$S$$ is reflexive, then $$0 \in S$$.
        If congruence modulo $$S$$ is symmetric,
        then $$S$$ is closed under taking additive inverses
        (i.e., if $$a \in S$$ then $$-a \in S$$).
        If congruence modulo $$S$$ is transitive,
        then $$S$$ is closed under addition.
  
    2.  We say that congruence modulo $$S$$ is *additive*
        if it has the property that,
        if $$a \equiv b \pmod{S}$$ and $$c \equiv d \pmod{S}$$, then $$a+c \equiv b+d \pmod{S}$$.
        
        Show: If congruence modulo $$S$$ is additive,
        then $$S$$ is closed under addition.
  
    3.  We say that congruence modulo $$S$$ is *multiplicative*
        if it has the property that,
        if $$a \equiv b \pmod{S}$$ and $$c \equiv d \pmod{S}$$, then $$ac \equiv bd \pmod{S}$$.
        
        Show: If congruence modulo $$S$$ is multiplicative,
        then $$S$$ absorbs products.
        
        (Hint: For $$r \in R$$ and $$f \in S$$,
        we have $$r \equiv r+f \pmod{S}$$ and $$f \equiv 0 \pmod{S}$$.)
    
    4.  Show: Congruence modulo $$S$$ is reflexive, symmetric, transitive, additive, and multiplicative
        if and only if $$S$$ is an ideal.
        
    In conclusion, we can use "modular arithmetic" in any ring, with respect to any ideal.
    This generalizes modular arithmetic of integers.
    One reason why ideals are important is because they are the subsets
    that make generalized modular arithmetic possible.



## Problems to complete on WebWork

No WebWork problems this week.



## Additional reading, required

You don't need to turn in anything for these tasks, but you do need to do them.

1.  Continue reading Chapter 2 of the textbook.

2.  Visit Herwig Hauser's [Gallery of Algebraic Surfaces](https://homepage.univie.ac.at/herwig.hauser/bildergalerie/gallery.html).
    These are surfaces, two-dimensional varieties, in $$\mathbb{R}^3$$,
    defined by a polynomial equation.
    
    Please take a look at the images there.
    Here are some questions for you to think about (but you do not have to answer them or turn in anything):
    
    1.  Do you have any favorite images in the gallery?
    
    2.  Did you see anything surprising or curious?
    
    3.  Some of the surfaces have "holes" while others don't.
        Some of the surfaces have "cusps", "pinches", or self-crossings, while others don't.
        Can you see any way to tell from the equation of a surface whether the surface will have
        any of those features?
        Do you think there is any way to tell that?
    
    4.  Are some of the surfaces similar? If so, are their equations similar?
        
        Are some of the equations similar? If so, are the surfaces similar?


## Additional reading, optional

+   Visit the Math Department's [publications](https://www.boisestate.edu/math/research/publications/),
    including undergraduate senior theses and the Senior Showcase,
    as well as graduate student master's theses.

+   Visit the Mathematics Colloquium web page: <https://www.boisestate.edu/math/research/colloquium/>

    Visit the Mathematics seminars web page: <https://www.boisestate.edu/math/research/seminars/>.
    Especially [TATERS](https://sites.google.com/boisestate.edu/taters/)
    will feature a lot of talks related to this class.

    You are invited to attend colloquium and seminar talks!

