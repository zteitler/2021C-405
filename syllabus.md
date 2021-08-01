---
layout: page
title: Syllabus
headercounters: true
mathjax: false
---

# Math 405/505, Fall 2021 Syllabus
{:.no_toc}

1. TOC
{:toc}


## Course Information

**Course Number**:
: Math 405 and 505

**Course Title**:
: Abstract Algebra

**Catalog Statement**:
: Topics in group theory, ring theory and field theory
  with emphasis on finite and solvable groups, polynomials and factorization,
  extensions of fields.


**Prerequisites**:
: MATH 301 and MATH 305


### Instructor

**Instructor**:
: Zach Teitler [he/him/his]

**Email**:
: <zteitler@boisestate.edu>

**Website**:
: <https://zteitler.github.io>

**Office**:
: MB 233A

**Office Phone**:
: 208-426-1086


### Section

**Section Number**:
: 001

**Meeting Times**:
: WeFr 10:30AM - 11:45AM

**Meeting Remotely**:
: We will meet remotely using Zoom.
  Zoom sessions may be recorded for students who are not able to attend.

**Zoom meeting ID**:
: TBA


## What this course is

This course is an introduction to abstract algebra
starting with rings, in particular polynomial rings.
We will focus on a part of algebra that has found widespread applications
throughout many areas of mathematics, sciences, and engineering:
computational algebra and algebraic geometry.
We will learn how the theory of algebra combines with computations,
and geometry,
to become a fascinating and surprisingly useful combination.

We'll learn about rings and ideals, focusing on ideals in polynomial rings.
One of the basic questions is to find a basis for a given ideal,
and in fact a basis with special properties called a Gröbner basis.
We'll learn why this is important,
how this can be used for a wide range of purposes,
and how it can be done in a practical way.
We'll touch on a range of applications including robotics,
but our primary application will be to elementary algebraic geometry,
which will get introduced along the way.
And in fact it's a two-way street,
with geometrical ideas circling back to inform the algebra and computations.

The central objects of our course will be
Gröbner bases (from algebra),
affine varieties (from algebraic geometry),
and the Buchberger algorithm.
We'll ask (and answer!) the basic questions:
what are they, how do they work,
and why are they important (and useful, and interesting).


### History and modernity

Algebraic geometry is among the oldest branches of mathematics,
standing on its own since the early 19th century
but with roots reaching back to the time of Euclid and Archimedes,
in the ancient Greek study of conics.


Over the course of its long history, algebraic geometry has developed strong connections
with many other areas of mathematics including
number theory, complex geometry, symplectic geometry, topology, model theory,
and especially abstract algebra.


In recent years there's been an unbelievable explosion of activity
in these areas, computational algebra, algebraic geometry,
and algorithms linking them.
These ideas now link to algebraic statistics,
phylogeny (biological descent),
chemical reaction networks,
tensors and machine learning,
and many more "applications".
This course will bring you to the threshold of a rapidly expanding,
and yet ever more interconnected,
world of mathematical and scientific ideas.

If you're planning to go on further in any area of math, science, or engineering,
being aware of computational algebra will help you
(and you might even end up using it directly!).
Even if you aren't, you will get to see one of the most successful
areas of math, and what great things can be accomplished by building up a little theory.
This course will give one of the nicest demonstrations I can think of
for why "pure", abstract math is so valuable.


### Solving systems of equations

In your linear algebra course you've learned about solving
*systems of linear equations* by methods such as row reduction.
This can be viewed from all three perspectives of our course:

Algebra:
: A system of equations is an algebraic thing, and can be approached
  by algebraic ideas such as manipulating and combining equations.

Geometry:
: Each linear equation defines a line or plane (or analogous object in higher dimensions).
  The central problem of solving a system corresponds to finding the intersection of the planes.

Algorithms:
: Row reduction, Gauss-Jordan elimination, and other procedures in linear algebra
  are algorithms: sequences of steps that allow us to do computations.

In our course, one of the basic starting points is to solve a
*system of non-linear, polynomial equations*.

+ Being a system of equations, we can use algebra to work with it.

+ Each equation will define a curve, surface, or in general, affine variety.
  Solving the system corresponds to finding the intersection of the varieties.

If these problems seem daunting, don't be afraid:

+ There are algorithms for working with systems of equations
  and affine varieties. Learning about these algorithms not only lets us
  answer questions about algebra and geometry, it also helps us
  *understand* those subjects more clearly.




## Course Learning Outcomes

By the end of this course, students will be able to:

1.  Demonstrate familiarity with concepts in ring theory and computational algebra,
    including rings, ideals, ideal bases, and Gröbner bases.

2.  Demonstrate familiarity with concepts in elementary algebraic geometry,
    including affine varieties, implicitization and parametrization of varieties,
    and operations on varieties including projection, union, and intersection.

3.  Demonstrate familiarity with computational algorithms
    for algebra and algebraic geometry including computation of Gröbner bases
    and projections of varieties.

4.  Explain connections between algebra, geometry, algorithms, and applications.

5.  Read and write rigorous proofs at an advanced level.

6.  Demonstrate good mathematical writing skills and style.



## Required Textbook

*Ideals, Varieties, and Algorithms*
    by David A. Cox, John B. Little, Donal O'Shea,
    Fourth Edition, 2015
    <https://dacox.people.amherst.edu/iva.html>




## Grading

### Components of course grade

The course grade will be based on written homework,
midterm and final exams, and a term paper.

### Homework

Homework will be written, weekly.
It will consist mostly of problems from the textbook,
plus some problems that I've written myself.
Most homework problems will be to write proofs,
but some will be computational (to compute certain things).

You are *strongly encouraged* to work collaboratively on homework
but you must turn in your own solutions.

In each homework set there will be some required problems (you have to turn them in),
and other problems will be a selection (try these problems, choose a certain number to turn in).

Your homework will be graded primarily on
(1) correctness and (2) writing quality (including clarity, explanation,
organization, etc.), but also, to a limited extent,
(3) the selection of which exercises to turn in.

#### Turning in written assignments

Homework submissions and grading will be paperless.
You will turn in your homework by uploading PDFs to Gradescope.

#### Homework format

Homework must be typed in LaTeX.
LaTeX tutorials are available online, e.g.,
<https://www.latex-tutorial.com> and <https://www.gnu.org/software/teximpatient/>.
You may wish to use a free online LaTeX system such as <https://overleaf.com>.
(Overleaf includes a LaTeX tutorial.)

Use a new page (`\newpage`) for each problem.
State which question you are answering
(textbook section and exercise number) and the actual question.
Then, start your answer in a new paragraph.

For legibility, use the `12pt` option
(`\documentclass[12pt]{amsart}`) and `\linespread{2.4}`.
If you use figures, I recommend learning to use `TikZ` to generate
high-quality figures within LaTeX.
Alternatively you may use figures/plots generated in other programs
such as Sage, Mathematica, Maple, or Inkscape, saved to PDF,
and included in your document with commands like `\includegraphics`.
It's also fine to include hand-drawn figures that you scanned or photoed.


### Midterm and final exams

A midterm exam in the 8th week of the semester,
and the final exam, will be individual oral exams.
The exams are intended to gauge mastery of course material,
as well as reflection on the course and its place in a larger context.



### Term Paper

Each student will write a term paper
about a topic of the student's choice within algebra or algebraic geometry.

1. An initial topic proposal (1-2 pages) is due by the end of week 4.
2. An outline is due by the end of week 6.
3. A first draft is due by the end of week 9.
4. A second draft is due by the end of week 12.
5. The term paper is due by the end of week 15.

The topic may be chosen from any source,
such as a section in the textbook that was not covered in class,
research literature, the *American Mathematical Monthly*, etc.
See also Appendix D of the textbook,
including in particular tutorials from the books by Kreuzer and Robbiano
(mentioned at the end of Appendix D).





### Attendance

Class attendance is **required** during the first week of the semester.
After the first week, because of the remote format of the course,
class attendance will be optional, not required, and not graded.
On the other hand it is *highly recommended*.
Attending class has many benefits such as:

+ Opportunities to ask questions and get immediate feedback
  (and then, ask followup questions).

+ Establish relationships with other students and with the instructor,
  which will be helpful in case you decide to look for a study group,
  research opportunities, or a letter of recommendation.



## Level of writing

One of the goals of this course is developing mathematical writing.
You are expected to meet high standards in mathematics and in writing,
but you can count on me to help you meet those standards.

Assignments should be well-written, with an appropriate level of detail.
This includes *mechanical* aspects of writing such as proof-reading for spelling,
punctuation, and grammar, *organizational* aspects such as use of complete sentences
and appropriate paragraphs, and especially *mathematical* aspects such as clarity,
conciseness, and of course correctness.
As a rule of thumb, proofs and computations should include
*sufficient detail to be clear to a typical student in this course*.

Elementary steps in computations and proofs may be omitted or carried out without comment,
while less obvious steps must be explained.
In particular, "computation" problems may often require a proof
of the correctness of the computation.


## Help

### Student times

I am here to support your learning.
I encourage you to meet with me when you feel that you need support or assistance.

In Fall 2021 I will be available:

**Student drop-in hours:**
: Thursdays 10:30am-12:30pm

**Student appointment hour:**
: Thursdays 12:30pm-1:30pm (email me to set up an appointment within this hour in 15-minute segments)

**Additional appointments:**
: Email me to set up an appointment on other days or times

Student times will be remote via Zoom
using my **office zoom link** (listed in Canvas, or email me for the link).



### Allowed resources

In this 400/500 level class,
you are encouraged to use the full array of resources available to you
to learn the material "by any means necessary".
For homework assignments, you are encouraged (in fact, expected)
to collaborate with your classmates and to ask me questions.
Other resources (books, online sources, people outside the class)
are highly recommended for clarifying class topics or for enrichment
(but not for getting solutions to problems).

You are allowed to use things that you learn from a book,
online source, or person outside the class that
help you and your classmates to find *your own solution* for a problem.
However, if you read a full solution, so that there's little or nothing
left for you and your classmates to figure out,
then you are not allowed to turn in that solution for credit.

### Helpful websites

The Mathematics Stack Exchange (<https://math.stackexchange.com>)
is a very useful question-and-answer site for undergraduate/graduate level mathematics.
You are welcome to browse the Mathematics Stack Exchange
and even post questions there.
Hopefully it will help you learn and understand the material!
However please remember that if you use that site to get a solution to a problem,
then you can't turn that solution in for credit.

Other helpful websites for basic math information include Wikipedia
and MathWorld (<http://mathworld.wolfram.com>).

### Textbook

See the textbook website <https://dacox.people.amherst.edu/iva.html>
for additional information,
including a list of mistakes ("errata")
which you may want to print out or save on your computer.

Additional suggested (optional) textbooks are listed on course website
page of [resources](resources).

### A note on collaboration

Solving mathematical problems has three parts:

1.  The discovery phase.
    
    This is the time you spent trying to figure out how to solve the problems,
    and it often takes most of the time.
    You are welcome and encouraged to collaborate with other students in this phase.
    Collaboration is a healthy practice, and this is how mathematics is done in real life.
    
    This phase starts with working to understand what a problem or question is asking for.
    That might include reviewing material from previous textbook sections.

2.  The write-up phase.
    
    This consists of writing your solutions once you have an idea
    of how the problem can be solved.
    You should do this entirely by yourself.
    Be alone when you write your solutions.
    If you collaborate on this part,
    or you copy part of your solutions from somebody else,
    or you have notes written by somebody else in front of you
    when you write your solutions,
    you are hurting yourself by depriving yourself of an opportunity to learn and practice.
    
    If you need help in the write-up phase, talk to me! I can help you.

3.  The editing phase.
    
    This consists of editing and revising your write-up for clarity,
    organization, and presentation.
    At this stage it can be very helpful to get feedback and suggestions
    from other students.


### University Resources

Boise State University's [The Basics](https://www.boisestate.edu/student-life/basics/)
web page has links to many forms of support,
ranging from academic resources to family, living, and food resources.

The Graduate College has
[many resources for graduate students](https://www.boisestate.edu/graduatecollege/current-students/)
such as GradWell,
the Graduate Student Success Center, and Graduate Writing Consultations,
as wells as forms, deadlines, and graduation information for graduate students.

Boise State University's
[Writing Center](https://www.boisestate.edu/writingcenter/)
may be helpful.

You may reach out to me at any time if there's anything I can help with
or if there's anything you think I should know.


## Important Dates

| Monday | 8/23 | First day of classes | 
| Monday | 9/3  | Last day to register/add or to drop without a W |
| Monday | 9/6  | Labor Day. No classes. |
| Friday | 9/17 | Term paper initial topic proposal is due (week 4) |
| Friday | 10/1 | Term paper outline is due (week 6) |
| Friday | 10/22 | Term paper first draft is due (week 9) |
| Friday | 10/29 | Last day to drop with a W or completely withdraw |
| Friday | 11/12 | Term paper second draft is due (week 12) |
|        | 11/22-28 | Thanksgiving Holiday. No classes. |
| Friday | 12/10 | Term paper final version is due (week 15) |
| Friday | 12/10 | Last day of instruction for regular classes |
| Wednesday | 12/15 | Final Exam, 12:00 p.m.-2:00 p.m. |
| Tuesday | 12/21 | Grades due. (You will be able to see your grade by this date.) |



## Other

**Respect for Diversity**:
: Students from all backgrounds and with all perspectives are welcome in this course.
  It is my intent that all students be well served by this course,
  that students's learning needs be addressed both in and out of class,
  and that the diversity that students bring to this class be viewed as a resource,
  strength, and benefit.
  It is my intent to maintain a classroom atmosphere that is welcoming and respectful
  of diversity: gender, sexuality, disability, age, socioeconomic status, ethnicity,
  race, and culture.
  Your suggestions are encouraged and appreciated.
  Please let me know ways to improve the effectiveness of the course for you personally
  or for other students or student groups.

**ADA Policy Statement**:
: Students with disabilities needing accommodations to fully participate in this class
  should contact the EAC.
  All accommodations must be approved through the EAC prior to being implemented.
  To learn more about the accommodation process, visit the EAC's website at
  <https://www.boisestate.edu/eac/new-students/>.

**Email**:
: In accordance with
  [Boise State University Policy #2280](https://boisestate.edu/policy/policy-title-student-e-mail-communications/),
  it is expected that you will receive and read emails sent to your `boisestate.edu`
  email address.

**Communication**:
: Additional information and updates may be announced in class, sent by email,
  and/or posted on BlackBoard (<https://blackboard.boisestate.edu/>).

**Academic Integrity**:
: Getting answers to homework or exam problems from unauthorized sources
  is a very serious form of academic misconduct.

**Behavioral Expectations**:
: Every student has the right to a respectful learning environment.
  In order to provide this right to all students, students must take
  individual responsibility to conduct themselves in a mature and appropriate manner
  and will be held accountable for their behavior in accordance with
  [Boise State University Policy #2050](https://boisestate.edu/policy/student-affairs/maintaining-order/).



