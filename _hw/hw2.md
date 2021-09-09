---
layout: assignment
title: Homework 2
duedate: 2021-09-15
mathjax: true
---

## Term paper

Please work on choosing a topic for your term paper.
A term paper "topic proposal" is due at the end of this week.

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


1.  Exercise 1.2.8.

2.  Exercise 1.2.13. It is optional to turn in part (a) (drawing a picture of the robot arm).
    You should draw a picture of the robot arm, but you don't have to turn in your picture.
    You do have to turn in parts b-d.

3.  Exercise 1.3.1.
    
    If you need to review linear algebra, please take the time to do so.
    Search for linear algebra, solving linear systems, and row operations
    on YouTube, Khan Academy, and the web.
    This is important background material that we will build on in Chapter 2,
    so if you need to review it, the time you spend will be worthwhile.

4.  Try to solve Section 1.3, Exercises 2, 3, 4, 5.
    Turn in the best/most interesting one that you are able to solve.

5.  Can $$16xy^3$$ be written as a fourth power? How about as a sum of fourth powers?
    In more detail:
    
    1.  Consider the equation
        \\[ (ax+by)^4 = 16xy^3. \\]
        Is there any solution for $$a,b$$?
        To answer this, expand the left hand side,
        and equate the coefficients of terms on each side of the equation.
        Write the system of equations for unknowns $$a,b$$ that make the above equation hold.
        For example, one of your equations will be $$a^4=0$$, corresponding to the coefficient
        of $$x^4$$ on each side; the coefficients of $$x^3y$$ lead to the equation $$4a^3b = 16$$.
        What are the other equations? Is there any solution for $$a,b$$?
        Does it make a difference what field is being used?
    
    2.  Consider the equation
        \\[ (ax+by)^4 + (cx+dy)^4 = 16xy^3. \\]
        Write the resulting system of equations for $$a,b,c,d$$.
        
        You do NOT need to try to solve this system.
        However do count the number of unknowns and the number of equations.
        Make a guess: do you think that this system probably has a solution,
        or probably doesn't have a solution?


{% comment %}
5.  The set $$\{\pm1\}^n$$ consists of sequences of length $$n$$ with entries $$\pm1$$.
    For $$\epsilon \in \{\pm1\}^n$$ we write $$\epsilon = (\epsilon_1,\dotsc,\epsilon_n)$$,
    so $$\epsilon_i$$ is the $$i$$th entry;
    we write $$\prod \epsilon$$ for the product $$\epsilon_1 \epsilon_2 \dotsm \epsilon_n$$.
    
    Let
    \\[
      P(x_1,\dotsc,x_n)
      = \sum_{\epsilon \in \{\pm1\}^n}
      \left(\prod \epsilon\right) (\epsilon_1 x_1 + \epsilon_2 x_2 + \dotsb + \epsilon_n x_n)^n .
    \\]
    
    1.  Find (and simplify) $$P(x_1,x_2)$$, $$P(x_1,x_2,x_3)$$, and $$P(x_1,x_2,x_3,x_4)$$.
    
    2.  What is $$P(x_1,\dotsc,x_n)$$ for all $$n \geq 2$$? Make a conjecture.
        Prove your conjecture if possible.
{% endcomment %}


## Problems to complete on WebWork

Visit [WeBWork](https://calculus.boisestate.edu/webwork2).
Complete the "Section 1.1" assignment within WebWork.


## Additional reading, required

1.  Read the rest of Chapter 1 of the textbook. Get ready to start reading Chapter 2.

2.  Read about "mathematical maturity":
    
    + <https://terrytao.wordpress.com/career-advice/theres-more-to-mathematics-than-rigour-and-proofs/>,
      by Terry Tao (Fields medalist).
      (Don't read the comments.)
      
    + <https://en.wikipedia.org/wiki/Mathematical_maturity>
    
    (You don't have to read this, but if you want to read a much, much longer discussion,
    there is one here: <http://iae-pedia.org/Math_Maturity>.)
    
    You don't have to turn in anything, but you are invited to reflect on these questions:
    
    + Which parts of "mathematical maturity" seem most important or valuable?
    
    + Which parts of "mathematical maturity" seem easy, or difficult, to acquire?
    
    + How would you assess someone's "mathematical maturity"?
    
    + Do you feel like you have "mathematical maturity"?
      Some parts of it? All?
      Do you feel that the math classes you have taken have contributed to
      your mathematical maturity growing?


## Additional reading, optional

+   A video playlist on [What are commutative algebra and algebraic geometry?](https://youtube.com/playlist?list=PL098oyLjkc7p__6t2COpfetDuhVsA3WCJ).
    What are commutative algebra and algebraic geometry,
    what do those subjects study, what kind of questions do they try to answer,
    and why are they interesting?
    The playlist also has a few more basic videos (what's a ring, what's an ideal)
    just to help you understand the terminology in the other videos.
    Most of the videos in this playlist are taken from the starts of playlists by other video creators,
    so if you see a video you like, you can follow up and learn more from that video creator.

+   Two videos about [graduate school in mathematics](https://youtube.com/playlist?list=PL098oyLjkc7q5QkD_bIuzT2s5HKim4qrJ)

+   Visit the Mathematics Colloquium web page: <https://www.boisestate.edu/math/research/colloquium/>

    Visit the Mathematics seminars web page: <https://www.boisestate.edu/math/research/seminars/>.
    Especially [TATERS](https://sites.google.com/boisestate.edu/taters/)
    will feature a lot of talks related to this class, including a talk by John Little, one of the textbook authors.

    You are invited to attend colloquium and seminar talks!

