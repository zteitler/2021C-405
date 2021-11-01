---
layout: assignment
title: Homework 7
duedate: 2021-11-03
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


1.  Section 3.1, Exercise 2, parts (a)-(c) (skip part (d)).
    
    Instructions:
    
    + Please do computations by hand. You can use a computer or calculator
      to check your work, and to help with arithmetic.
    
    + You do not have to type the steps of divisions in LaTeX. Instead, show
      the result of the division, the remainder, for example "When we divide
      $$x^2$$ by $$G_1$$ the remainder is $$y+1$$."

2.  Let $$X = \begin{pmatrix} x_1 & x_2 & x_3 \\ x_4 & x_5 & x_6 \end{pmatrix}$$.
    Let $$R = \Bbbk[x_1,\dotsc,x_6]$$ with lex order with $$x_1 > \dotsb > x_6$$.
    Let $$G = \{ x_1 x_5 - x_2 x_4, x_1 x_6 - x_3 x_4, x_2 x_6 - x_3 x_5 \}$$.
    (Notice that these are the determinants of $$2 \times 2$$ submatrices of $$X$$.)
    Is $$G$$ a Gröbner basis?

3.  This problem is canceled.

Let $$R$$ and $$S$$ be rings (commutative rings with $$1$$).
A *homomorphism* from $$R$$ to $$S$$ is a function $$f : R \to S$$
that "respects" the ring operations, meaning:
+ $$f(r_1+r_2) = f(r_1) + f(r_2)$$ for all $$r_1,r_2 \in R$$,
+ $$f(r_1r_2) = f(r_1) f(r_2)$$ for all $$r_1,r_2 \in R$$, and
+ $$f(1_R) = 1_S$$.

(Here, the operations $$r_1+r_2$$ and $$r_1 r_2$$ in the inputs to $$f$$
are the addition and multiplication in $$R$$,
while the operations $$f(r_1)+f(r_2)$$ and $$f(r_1)f(r_2)$$
are the addition and multiplication in $$S$$.)

{: start="4"}
4.  Suppose $$f : R \to S$$ is a homomorphism.
    Prove the following.
    
    1.  $$f(0_R) = 0_S$$  
        (Hint: Use $$0_R+0_R=0_R$$ and the homomorphism property of $$f$$,
        then subtract something from both sides.)
    
    2.  $$f(-r) = -f(r)$$ for all $$r \in R$$  
        (Hint: Use $$r+(-r)=0_R$$ and the homomorphism property of $$f$$.)
    
    3.  The *kernel* of $$f$$ is defined by $$\ker(f) = \{ r \in R \mid f(r) = 0\}$$.
        Prove that the kernel of $$f$$ is an ideal in $$R$$.  
        (Hint: Show that the kernel of $$f$$ satisfies the definition of an ideal.)

5.  Prove the following.

    1.  If $$f : R \to S$$ and $$g : S  \to T$$ are  homomorphisms,
        then so is $$g \circ f : R \to T$$.  
        (Hint: Show that $$g \circ f$$ has the homomorphism properties.)
    
    2.  If $$f : R \to S$$ is a homomorphism and $$f$$ is a bijection (one-to-one and onto),
        then $$f^{-1}$$ is also a homomorphism.  
        (Hint: Show that $$f^{-1}$$ has the homomorphism properties.
        Given $$s_1,s_2 \in S$$, we can write $$s_1=f(r_1), s_2=f(r_2)$$
        for some $$r_1,r_2 \in R$$ (why?).
        Use the homomorphism properties for $$f$$ with $$r_1,r_2$$
        to show the homomorphism properties for $$f^{-1}$$ with $$s_1,s_2$$.)
        


## Problems to complete on WebWork

No WebWork problems this week.



## Additional reading, required

You don't need to turn in anything for these tasks, but you do need to do them.

1.  Continue reading Chapter 3 of the textbook.



## Additional reading, optional


+   Visit the Mathematics Colloquium web page: <https://www.boisestate.edu/math/research/colloquium/>

    Visit the Mathematics seminars web page: <https://www.boisestate.edu/math/research/seminars/>.
    Especially [TATERS](https://sites.google.com/boisestate.edu/taters/)
    will feature a lot of talks related to this class.

    You are invited to attend colloquium and seminar talks!

