---
layout: assignment
title: Term paper, first draft
duedate: 2021-11-05
mathjax: true
---

Write a first draft of your term paper.

## Purpose

The purpose here is two-fold:

1. Have an opportunity for feedback and suggestions.

2. Making sure you stay on schedule to finish a term paper
   without a big rush at the end of the semester.

3. Peer review to give each other feedback and share ideas.
   
## Assignment

Write a first draft of your term paper.
Use LaTeX and make a PDF.
Upload your PDF to **Canvas**.


## Requirements

Given the realities of an academic semester,
your term paper first draft is allowed to be
an _incomplete draft_.
Here is what is required:

1. Your paper should have a title and identifiable topic/theme.
   It should include your name as the author.

2.  Create **sections** in your paper using `\section{...}`,
    for example `\section{Introduction}`, `\section{Main Theorem}`, etc.

2.  Your paper is allowed to be **incomplete**. It does _not_ need to have all sections written.
    However your paper should include **at least one section that is complete, or nearly complete**.
    
    + _Recommendation_: The (nearly) complete section should be
      one of the main content sections, with the main theorems or highlights
      of your paper.
      It should not be the Introduction or the background section.
      Those are important too, but not a good place to start your writing,
      because they can change a lot if the main sections change.
      Therefore I recommend to get the main sections figured out and written first.
      
      
3.  Try to include at least one theorem statement and at least one proof.
    
    + This could be a smaller result such as a lemma or corollary
      but ideally it would be one of the main results.
      
    + At this stage the proof can be incomplete.
    

4.  Include a bibliography with at least one reference.
    See ["How to Bibliography"](https://zteitler.github.io/assets/how-to-bibliography-2.pdf)
    for information.
    
    For this draft, don't worry about formatting.
    Proper formatting will be added in the second draft.
    
5.  Use LaTeX to produce a PDF with reasonable formatting,
    similar to homework.
    
    + _Readability_: Please use reasonable margins (at least 1 inch),
      a 12-point option such as `\documentclass[12pt]{amsart}`,
      and `\linespread{2.4}` to produce something like double-spaced lines.
    
    + _LaTeX Environments_: Please use LaTeX environments such as
      `\begin{theorem}...\end{theorem}`, `proof`, etc.
      See for example
      [Overleaf's tutorial on theorems and proofs](https://www.overleaf.com/learn/latex/theorems_and_proofs).

## Advice

Finally, some advice (not required).
A normal part of the writing process is to realize that your plans and goals
were too ambitious.
If you start to feel that you have taken on too large of a writing task,
some options that you might consider include:

+ _Focus on a special case of your main result._
  For example, instead of $$n$$ dimensions,
  just deal with the $$1$$ or $$2$$ dimensional case.
  (Better yet, start with the "trivial"/"easy" cases,
  and then focus on the *first non-trivial case*.)
  You might just briefly discuss the more general case,
  or just state it, or even just give a citation to it;
  or maybe not get into it at all.
  
+ _Omit some technical or difficult things._
  Don't skip over the main points of proofs, or the important things
  that are the reason your topic is interesting.
  Keep those important steps.
  But there might be other steps that can be cut while still
  conveying all the important points.

+ _Pick a running example._
  This can be used to illustrate or demonstrate some results,
  or some steps, when the general case is too difficult.
  This might require two or more examples.

+ _You can expect something from your reader._
  Don't feel that you have to explain every single thing
  to the reader.
  You can expect them to know _something_.
  To play it safe, you can "recall" specific facts that you need.

A final piece of advice is

+ _Don't get bogged down in introductory or trivial things._
  It can make a very good paper to include some introduction, context, history, etc.,
  and also to explain a simple or trivial case,
  in order to illustrate by contrast what makes other cases difficult or non-trivial.
  Proving your main theorem in this case can help the reader appreciate
  the non-trivial cases.
  
  However, don't get bogged down in this.
  If the main point of your paper is the non-trivial case, then keep that in mind,
  treat the easier case as just setup for the main point,
  and get to the main point.
