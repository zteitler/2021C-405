---
layout: assignment
title: Homework 9
duedate: 2021-11-17
mathjax: true
published: true
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


## Using a computer for computations

On this homework you are allowed to use a computer to do some of the long
computations with Gröbner bases.
Take a look at [basic directions to help you get started]({{ "/computing" | relative_url }}).


## Problems to turn in on Gradescope

1.  Choose one of Exercise 2.8.2 or Exercise 2.8.4.

2.  Exercise 2.8.11.
    
    (This exercise is an example of a pattern.
    If $$a+b+c=3$$, $$a^2+b^2+c^2=5$$, and $$a^3+b^3+c^3=7$$,
    then we see a pattern that each time the powers increase we get the next odd number.
    And indeed, from those given values, we can show that $$a^4+b^4+c^4=9$$.
    With such a strong pattern, anyone would predict $$a^5+b^5+c^5$$ must be equal to $$11$$.
    But is it?)
    
    Hint: If you can show that $$a^4+b^4+c^4-9$$ is in the ideal
    $$\langle a+b+c-3, a^2+b^2+c^2-5, a^3+b^3+c^3-7 \rangle$$,
    so
    
    $$ a^4+b^4+c^4-9 = (a+b+c-3)q_1 + (a^2+b^2+c^2-5)q_2 + (a^3+b^3+c^3-7)q_3 $$
    
    for some $$q_i$$ (it doesn't matter if you actually find the exact $$q_i$$)
    then, from the given information that $$a+b+c=3$$, $$a^2+b^2+c^2=5$$, etc.,
    the right hand side will be equal to zero.
    What does that mean for the left hand side?
    What does it mean for the value of $$a^4+b^4+c^4$$?
    
    What would it mean if there was a remainder?

3.  A polynomial $$F \in R = \Bbbk[x_1,\dotsc,x_n]$$
    is called *homogeneous* of degree $$d$$
    if every term of $$F$$ has total degree equal to $$d$$.
    
    For example, if $$F = x^4y + x^2z^3 + xyz$$,
    and we wanted to write $$F = F_5 + F_4 + F_3$$ where each $$F_i$$ was homogeneous of degree $$i$$,
    it would be $$F_5 = x^4y + x^2z^3$$, $$F_4 = 0$$, and $$F_3 = xyz$$.
    
    We write $$R_d$$ for the set of homogeneous polynomials of degree $$d$$,
    together with the zero polynomial.
    
    Try to prove all of the following.
    Turn in the best three (3) that you are able to prove.
    
    1.  If $$F$$ and $$G$$ are homogeneous of the same degree $$d$$,
        then so are $$F+G$$ and $$\lambda F$$ for all $$\lambda \in \Bbbk$$.
        (Thus $$R_d$$ is a vector space.)
    
    2.  If $$F$$ is homogeneous of degree $$d$$ and $$G$$ is homogeneous of degree $$e$$,
        then $$FG$$ is homogeneous of degree $$d+e$$.
    
    3.  If $$F$$ is nonzero and homogeneous of degree $$d$$,
        and $$FG$$ is homogeneous of degree $$d+e$$,
        then $$G$$ is homogeneous of degree $$e$$.
        
        (Hint: Write $$G = G_0 + G_1 + \dotsb + G_k$$,
        where each $$G_i$$ is homogeneous of degree $$i$$,
        by grouping together terms.
        Then $$FG = FG_0 + FG_1 + \dotsb + FG_k$$.)
    
    4.  Find a basis for $$R_d$$.
        Find and prove a formula for the dimension of $$R_d$$
        (in terms of the degree $$d$$ and the number of variables $$n$$).



4.  Let $$F \in S = \mathbb{C}[x_1,\dotsc,x_n]$$.
    Let $$T = \mathbb{C}[y_1,\dotsc,y_n]$$.
    We can treat $$T$$ as an ordinary polynomial ring,
    just with different symbols for the variables ($$y$$ instead of $$x$$).
    But we can also think of elements of $$T$$ as differential operators,
    where $$y_i$$ stands for $$\frac{\partial}{\partial x_i}$$.
    When elements of $$T$$ act on elements of $$S$$,
    let's denote it with the symbol $$\circ$$ (`\circ`), as in
    $$y_i \circ x_i^d = d x_i^{d-1}$$;
    $$y_1 y_2^3 \circ x_1^5 x_2^7 x_3 = 5 \cdot (7 \cdot 6 \cdot 5) x_1^4 x_2^4 x_3$$;
    $$(3 y_1 - 5 y_2) \circ x_1^3 x_2^7 = 3 \cdot 3 x_1^2 x_2^7 - 5 \cdot 7 x_1^3 x_2^6$$;
    and so on.
    
    Let $$F^\perp = \{ \Theta \in T \mid \Theta \circ F = 0 \}$$.
    
    Try to prove all of the following.
    Turn in the best two (2) that you are able to prove.
    
    1.  Prove that $$F^\perp \subseteq T$$ is an ideal.
    
    2.  Explain why if $$F$$ has degree $$d$$, then every monomial of degree $$d+1$$
        is in $$F^\perp$$.
        Find $$V(F^\perp)$$.
    
    3.  Suppose $$n=2$$.
        Prove that if $$F = x_1^{a_1} x_2^{a_2}$$ is a monomial, then
        $$(x_1^{a_1} x_2^{a_2})^\perp = \langle y_1^{a_1+1},y_2^{a_2+1} \rangle$$.
        (Optional: What about monomials in $$n$$ variables for $$n > 2$$?)
    
    4.  Suppose $$n=2$$.
        Prove $$(x_1^d + x_2^d)^\perp = \langle y_1^d-y_2^d, y_1 y_2 \rangle$$.
        
        Hint: You can check $$(y_1^d-y_2^d) \circ (x_1^d+x_2^d) = 0$$
        and $$(y_1 y_2) \circ (x_1^d+x_2^d) = 0$$, which means
        $$y_1^d-y_2^d \in (x_1^d+x_2^d)^\perp$$ and $$y_1 y_2 \in (x_1^d+x_2^d)^\perp$$.
        
        Next, find a Gröbner basis for the ideal on the right hand side.
        Suppose $$\Theta$$ is any element of the left hand side.
        To show that $$\Theta$$ is in the right hand side, divide $$\Theta$$ by the Gröbner basis.
        What can the remainder be; specifically, what monomials can appear in the remainder?
        Explain why the remainder is also in the left hand side.
        Use the information about the remainder to show that the remainder must be equal to zero.


Finally choose one (1) of the following two problems to turn in.

{: start="5"}
5.  Redo one (1) problem from a previous homework.

6.  This exercise introduces maximal ideals
    and shows some examples of maximal (and non-maximal) ideals.
    The idea of maximal ideals will play an important role in Chapter 4.
    
    *Definition.* For a ring $$R$$,
    an ideal $$I \subset R$$ is called a **maximal** ideal of $$R$$ if
    
    + $$I \neq R$$ ($$I$$ is a proper ideal of $$R$$), and
    
    + for any ideal $$J$$ such that $$I \subseteq J \subseteq R$$,
      we have $$J=I$$ or $$J=R$$.
      That is, $$I$$ is as large as possible, for a proper ideal;
      no proper ideal can possibly contain $$I$$, except for $$I$$ itself.
    
    (It is equivalent to say: $$1 \notin I$$ and if $$I \subsetneq J$$, then $$J = R$$.
    Or in other words: $$1 \notin I$$ and if $$I \subset J$$
    and there is an element $$p \in J$$, $$p \notin I$$, then $$1 \in J$$.
    This means you can show an ideal $$I$$ is maximal
    by showing $$1 \notin I$$ and, if $$J$$ is any ideal such that $$I \subset J$$
    but there is some element $$p \in J$$, $$p \notin I$$, then $$1 \in J$$.)
  
    Prove the following facts about maximal ideals.
    
    1.  Let $$\Bbbk$$ be any field,
        let $$R = \Bbbk[x_1,\dotsc,x_n]$$,
        and let $$a = (a_1,\dotsc,a_n) \in \Bbbk^n$$.
        Let $$\mathfrak{m}_a = \langle x_1-a_1,\dotsc,x_n-a_n \rangle$$.
        Show that $$\mathfrak{m}_a$$ is a maximal ideal of $$R$$.
        (`\mathfrak{m}_a`)
        
        This exercise shows that every point in $$\Bbbk^n$$ gives us a maximal ideal.
    
    2.  Let $$\Bbbk$$ be any field and let $$R = \Bbbk[x_1,\dotsc,x_n]$$.
        Let $$I \subseteq R$$ be an ideal and let $$a = (a_1,\dotsc,a_n) \in \Bbbk$$.
        Then $$(a_1,\dotsc,a_n) \in V(I)$$ if and only if $$I \subseteq \mathfrak{m}_a$$.
    
    3.  Let $$R = \mathbb{R}[x]$$, and let $$I = \langle x^2+1 \rangle$$.
        Show that $$I$$ is a maximal ideal of $$R$$. What is $$V(I)$$?
    
    This shows that maximal ideals can have other forms
    besides corresponding to points in $$\Bbbk^n$$.
    
    {: start="4"}
    4.  Now show that $$\langle x^2+1 \rangle \subset \mathbb{C}[x]$$
        is *not* a maximal ideal.
    
    5.  Show that $$(x^2+2+\sqrt{2})(x^2+2-\sqrt{2}) = x^4+4x^2+2$$
        and $$\langle x^4+4x^2+2 \rangle$$
        is a maximal ideal in $$\mathbb{Q}[x]$$,
        an intersection of two maximal ideals in $$\mathbb{R}[x]$$,
        and an intersection of $$4$$ maximal ideals in $$\mathbb{C}[x]$$.
    
    It turns out that when $$\Bbbk$$ is an algebraically closed field,
    maximal ideals correspond to points;
    over non-algebraically closed fields, there can be "extra" maximal ideals.


## Problems to complete on WebWork

No WebWork problems this week.



## Additional reading, required

You don't need to turn in anything for these tasks, but you do need to do them.

1.  Read the first few sections of Chapter 4 of the textbook.
    The textbook's proof of Hilbert's Nullstellensatz won't be covered in class
    (we'll give a different proof).



## Additional reading, optional

+   Read in the textbook about Bezier curves.

+   [Are there any practical uses of algebraic geometry?](https://www.quora.com/Are-there-any-practical-uses-for-algebraic-geometry-outside-of-someone-s-profession)
    and Wikipedia's [Applications of algebraic geometry](https://en.wikipedia.org/wiki/Algebraic_geometry#Applications)


+   Visit the Mathematics Colloquium web page: <https://www.boisestate.edu/math/research/colloquium/>

    Visit the Mathematics seminars web page: <https://www.boisestate.edu/math/research/seminars/>.
    Especially [TATERS](https://sites.google.com/boisestate.edu/taters/)
    will feature a lot of talks related to this class.

    You are invited to attend colloquium and seminar talks!

