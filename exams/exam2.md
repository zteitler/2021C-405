---
title: Exam 2
layout: page
mathjax: true
---

# Exam 2

## Exam rules

The exam is modeled on
<https://mathinthetimeofcorona.wordpress.com/2020/06/11/june-11-day-95-finals-part-ii/>.

You can use all available resources to prepare, including but not limited to:
each other, books, notes, the internet.
During the exam, however, please use only a single 8.5x11 sheet of notes.
{% comment %}
Your true/false questions for question 1 don't count toward the sheet of notes
(you can have a sheet of notes in addition to your true/false questions).
{% endcomment %}

You will have 20 minutes to answer **two questions**.
The first question will be your choice and the second will be mine.
Since you don't know which question I will choose, you should prepare answers to all the questions.

However, you may reject my chosen question, and I will choose a different one.
So it's okay if there are one or two questions that you don't want to answer.
If you reject my chosen question, there will be a 4 point reduction in your score.
You can reject my chosen question twice (limit of 2 times).


At the end of the exam I will ask you for a self-assessment of your performance.



During the exam we will talk in a conversational style.
As part of this I will ask you to turn on your microphone and camera.

Please be prepared to present your work, including responding to questions.
The following formats are suggested:
+ Writing on a tablet screen using a stylus
+ Writing on paper with a document camera
+ Writing on a chalkboard or whiteboard

Prepared slides may be part of your presentation, but they are not well suited
for responding to questions where your response might involve writing.
So even if you include slides, please be prepared to also use one of the above formats.
If it will not be possible for you to use any of the above,
please let me know in advance.


## Questions

You should prepare answers to all the questions (or, as many as you can).
However, during the exam you will answer two questions.

1.  Describe one thing you learned in this course about rings, ideals, and algebra,
    one thing you learned about varieties and geometry,
    and one thing you learned about algorithms and computation.
    Explain why the things you chose are interesting, useful, or important.

2.  Of the written homework you submitted this term,
    choose a problem that you found challenging,
    critique your original written submission,
    and present an improved solution.
    In the context of this problem, describe the challenge, how you overcame it,
    and how it was valuable to you.

3.  Textbook exercise 2.8.8

4.  Textbook exercise 2.7.10 (relating to linear algebra)
    or textbook exercise 2.7.14 (relating to interpolation).

5.  A radical ideal:
    
    1.  Using the division algorithm, explain why any $$f \in k[x,y]$$ can be written as
        
        $$ f = g(x,y) \cdot (x^2-1) + h(x,y) \cdot y + r(x), $$
        
        where $$\deg(r) \leq 1$$.
    
    2.  Let $$V = \{(1,0), (-1,0)\} \subset k^2$$. Prove that $$I(V) = \langle x^2-1,y \rangle$$.
        
        _Hint:_ Prove that $$x^2-1,y \in I(V)$$.
        Prove that if $$f \in I(V)$$ then $$r \in I(V)$$, where $$r$$ is defined as in the previous part.
        Prove that if $$\deg(r) \leq 1$$ and $$r(1)=r(-1)=0$$, then $$r = 0$$.
    
    3.  Let $$I = \langle x^2+y^2-1, 3x^2+y^2-3 \rangle$$. Find $$V(I)$$.
    
    4.  State a version of the Nullstellensatz that relates to radicals of ideals,
        and use it to find the radical $$\sqrt{I}$$.
    
    5.  Are $$x^2-1,y \in I$$? Find integers $$m$$ and $$n$$ so that $$(x^2-1)^m \in I$$
        and $$y^n \in I$$.

6.  Let $$R = k[x_1,\dotsc,x_n]$$ and let $$I,J \subseteq R$$ be ideals.
    We define the _ideal quotient_ $$I:J$$ as follows:
    
    $$ I:J = \{ f \in R \mid \text{for all } g \in J, fg \in I \}. $$
    
    1.  Prove that $$I \subseteq I:J$$. Explain why this implies $$V(I:J) \subseteq V(I)$$.
    
    2.  Prove that $$V(I)-V(J) \subseteq V(I:J)$$.
        
        (Here the subtraction means the set difference, in other words
        elements of $$V(I)$$ that are not in $$V(J)$$.)
        
        _Hint:_ Suppose $$a \in V(I)-V(J)$$.
        There is some $$g \in J$$ such that $$g(a) \neq 0$$ (why?).
        Let $$f \in I:J$$.
        Use $$fg \in I$$ and $$a \in V(I)$$ to prove $$f(a)=0$$.
    
    3.  Prove that $$I:J$$ is an ideal.
    
    4.  Prove one (1) of the following. (State clearly which one you are proving.)
        
        1.  If $$J_1, J_2$$ are two ideals such that $$J_1 \subseteq J_2$$,
            then $$I : J_1 \supseteq I : J_2$$.
        
        2.  If $$J_1, J_2$$ are two ideals, then $$I:(J_1+J_2) = (I:J_1) \cap (I:J_2)$$.
        
        3.  If $$I_1, I_2, J$$ are ideals, then $$(I_1 \cap I_2):J = (I_1:J) \cap (I_2:J)$$.

## Grading

Questions will be graded out of 50 points (each) using the following rubric
(copied from the web page linked above).

| A | 50 | Well-executed, well-communicated, essentially correct. Minor errors quickly corrected. No nontrivial errors. |
| B | 43 | Generally well-executed. Some minor errors not recognized or corrected. Nontrivial errors corrected when identified. |
| C | 38 | Adequately executed but numerous or repeated errors (minor and nontrivial) without satisfactory resolution. |
| D | 33 | Flawed execution with nontrivial errors. |
| F | 25 | Unsatisfactory execution with fundamental errors and deep misunderstandings. |
| 0 |  0 | Very little of relevance. No evidence of preparation. |

Since there are two questions graded out of 50 points each,
the exam total score is out of 100 points.

## Scheduling

You will schedule an online, one-on-one meeting with me for the exam.
Meetings will be scheduled for half-hour blocks either from :00 to :30, or :30 to :00.
Exams are expected to take 20 minutes;
the extra time is for safety, in case of delay or technical difficulties.

Available meeting times are:


| Monday, December 13 | 9:30-11:00am |
| Tuesday, December 14 | 11:00am-2:30pm |
| Wednesday, December 15 | 11:00am-2:30pm |
| Thursday, December 16 | 9:30am-12:00pm, 12:30pm-2:30pm |

You can reserve an exam time with a
[Google Calendar appointment](https://calendar.google.com/calendar/u/0/selfsched?sstoken=UUxMOE5iZlhHc2dMfGRlZmF1bHR8NjI5MDgyNTcxYWExZGRhZjJhMDY1Y2UyYzI2YjEzODM).

If other days/times are needed, please contact me.


## Time limit

Due to the number of enrolled students, it is not possible to extend exam times.
It will be very important for you to have your answers prepared and rehearsed;
thinking through an answer on the spot is not recommended.

There will be about 10 minutes for each question.
As a guideline, plan to spend about 5 minutes giving your prepared answer,
then 5 minutes on discussion and follow-up questions.
Please don't prepare answers that will take much longer than 5 minutes.
For a discussion/reflection question, this means preparing a short, focused answer,
with just a few carefully selected examples.
For a proof question, this might mean preparing a summary or overview of the key steps
of the proof, not trying to present every single detailed step.

This can be challenging (it's hard enough trying to figure out a tricky proof,
even harder to present it, and then much harder with a strict time limit on top of that).
For what it's worth, focused and to-the-point communication is an important skill.
Some tips include:

+   Work together with other students to plan and practice your answers.

+   Decide in advance which question you will choose to answer,
    and which questions you will reject if I choose them.
    (Don't use up your time deciding this during the exam!)

+   You can assume that I am familiar with the questions and with basic definitions.
    You do not need to repeat the question, or repeat the definitions of basic terms
    (unless there's some detail that's important for your answer).
    Once you've told me what question you want to answer
    (or, once I've told you what question I want you to answer),
    you can simply begin answering it.

+   Personally, I enjoy clear, well-prepared, well-executed answers, even if they are
    for "easy" questions.
    (But if you want to answer a challenging question, that's fine too!)
    
    That means you should choose a question that you can answer well, even if it's "easy,"
    rather than trying to impress me with a "difficult" question that you can barely answer.


+   Think about what follow-up questions might be asked.
    Some possibilities include: asking you to expand on a detail of your prepared answer;
    a "what-if" question asking you for a different version of the main question
    (e.g., "what if we used a different monomial order?");
    asking how you would teach the answer you just gave.
    As part of your preparation, think about how you might handle these or other questions.
    
+   Don't write down or memorize answers to every possible follow-up question.
    It's okay to think about the follow-up questions during the exam.
    In fact, that's a good thing, since it shows your thought process.
    The point of thinking about possible follow-up questions ahead of time
    is just to be prepared and calm during the exam.


+   Think about what needs to be written down as part of your presentation and what can
    be simply said out loud.
    Given the format of the exam (remote over Zoom, with a time limit),
    the less you need to write down, the better and easier it will be for you to explain your answers
    without having to rush or handle awkward writing situations.
    
    The exam is a conversation between two people: you and me.
    Please feel free to talk like a person having an ordinary conversation.
    
    There may be some things that simply have to be written down,
    but there's a lot that can simply be said, maybe more than you might be guessing.


## How to prepare

I encourage you to work together with other students in the class to plan and practice your answers.
*I want you to work together. This is the whole point of setting up the exam in this way.*
Solve the exercises together.
Work together to think of examples.

Please choose different examples
(don't all show up with the exact same example of how
a system of polynomial equations arises in science).
But you should share your examples with each other,
to help each other think of examples,
and also to get feedback how your example can be improved.

Practice your answers, including using a timer and asking each other follow-up questions.
(In a friendly way!)
