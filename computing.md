---
layout: page
title: Computing
headercounters: true
mathjax: true
---

# Computing with computers

## Introduction

In our class we've learned about polynomial division, the Buchberger algorithm,
and other algorithms for computing with polynomials.
Experience shows that it doesn't take much for the computations to exceed
what we can possibly do by hand, without a computer.
Fortunately, there are several computer algebra systems (CAS) that can do these algorithms.

This page will give just a few of the free options and some very basic instructions
to help you get started.
Material on this page is drawn from various sources including
[Greg Smith's Macaulay2 worksheet](https://mast.queensu.ca/~ggsmith/Math413/macaulay2.pdf).

For our class you are not required to download and install any software to your computer.
You are not required to use any of this software or learn it.
However it is recommended, as it can help you with some homework problems.
If you don't want to learn or use this software, you should work with a group of students
who can help you.

### Recommendation

If you are already familiar with Sage and Python,
you can use it for polynomials as well, and you won't have to learn a new system.

Otherwise, the easiest to learn is probably Macaulay2 (but that's subjective).
I recommend starting with Macaulay2.
If you don't like it, try Sage.

For most students just getting started, the Singular interface will be pretty unfamiliar.
If you are new to computer algebra systems or computer programming,
it might be easier for you to try using Macaulay2 or Sage instead of Singular.




## [Macaulay2](https://faculty.math.illinois.edu/Macaulay2/)

Macaulay2 is free and open source.

### Try it online

You can try Macaulay2 online at <https://www.unimelb-macaulay2.cloud.edu.au/#home>,
or download and install it on your computer following directions
at the [Macaulay2](https://faculty.math.illinois.edu/Macaulay2/) web site.

### Some basic commands

Try

```
2+2
2*2
2^2
4/2
4//2
100//7
100%7
(100//7)*7 + (100%7)
2+2 -- if you type "--" then the rest of the line is a comment (ignored by Macaulay2)
```

### Basic rings and ideals

Try

```
R = QQ[x,y] -- Ring with rational coefficients (QQ = \mathbb{Q}) and variables x,y
f1 = x+y-3
f2 = x^2+y^2-5
x*f1 - f2  -- this is S(f1,f2)
I = ideal(f1, f2)
G = gb I -- compute Grobner basis
ideal gens G -- show the generators in the Grobner basis
```

### Polynomial division

Unfortunately the default division algorithm in Macaulay2 is slightly different
from the simplified algorithm presented in the textbook.
Here is a Macaulay2 implementation of the exact division algorithm from the textbook
(adapted from code by Greg Smith).

```
ivadivision = (f,G) -> (  -- f is a polynomial and G is a list of polynomials
  S := ring f;
  p := f;
  r := 0_S;
  m := #G;
  Q := new MutableList from (m:0_S);
  for j from 0 to m-1 do Q#j = 0_S;
  while p != 0 do (
    i := 0;
    while i < m and leadTerm(p) % leadTerm(G#i) != 0 do i = i+1;
    if i < m then (
      Q#i = Q#i + (leadTerm(p) // leadTerm(G#i));
      p = p - (leadTerm(p) // leadTerm(G#i))*(G#i);
    ) else (
      r = r + leadTerm(p);
      p = p - leadTerm(p);
    )
  );
  return (r,toList Q);
);
```

To use this, enter the above code into Macaulay2.
Then you can use it like the following example.

```
f = x^2*y
G = {x^2-y, x*y-x}
ivadivision(f,G)
```

This will show the remainder when $$f$$ is divided by $$G$$,
followed by the quotient polynomials (the $$q_i$$ polynomials).
To extract just the remainder, use:

```
r = first ivadivision(f,G)
```

(If you are curious, you can see the results of Macaulay2's builtin division and remainder
algorithms with `f // matrix{G}` and `f % matrix{G}`.
You can see that they are different from the textbook algorithm.)

### Choosing different monomial orders

Different monomial orders can be chosen in Macaulay2 when the ring is created, with:

```
R = QQ[x,y,z, MonomialOrder=>Lex] -- lex order
R = QQ[x,y,z, MonomialOrder=>GLex] -- grlex order (the textbook calls it grlex, Macaulay2 calls it GLex)
R = QQ[x,y,z, MonomialOrder=>GRevLex] -- grevlex order
```


## [Sage](https://sagemath.org)

### Try it online

Sage can be tried online with CoCalc or SageMathCell,
both linked from the [Sage home page](https://sagemath.org).

### Polynomials

All the basic operations with polynomials can be performed in Sage.
I will try to add directions later.

### Polynomial division

Unfortunately the default division algorithm in Sage is slightly different
from the simplified algorithm presented in the textbook.
Here is a Sage implementation of the exact division algorithm from the textbook
(adapted from code by Greg Smith).

```
def ivadivision(f,G):
  R = parent(f)
  p = f
  r = R(0)
  m = len(G)
  Q = [R(0)]*m
  
  while (p != R(0)):
    dividingi = -1
    for i in range(m):
      if ( R.monomial_divides(G[i].lm(),p.lm()) ):
        dividingi = i
        break
    
    if ( dividingi == -1 ):
      r = r + p.lt()
      p = p - p.lt()
    else:
      Q[dividingi] = Q[dividingi] + R.monomial_quotient(p.lt(),G[i].lt(),coeff=True)
      p = p - R.monomial_quotient(p.lt(),G[i].lt(),coeff=True) * G[i]
  
  return [r,Q]
```


## [Singular](https://www.singular.uni-kl.de)

Singular is a powerful system.
The algebra in Sage uses Singular, just with a Sage interface.
Even Macaulay2 uses Singular for some routines
(technically, I believe Macaulay2 uses some libraries from Singular, not the whole Singular program).
However for most students just getting started, the Singular interface will be pretty unfamiliar.
If you are new to computer algebra systems or computer programming,
it might be easier for you to try using Macaulay2 or Sage instead of Singular.



### Try it online

Singular can be [tried online](https://www.singular.uni-kl.de:8003).
It can also be downloaded and installed on your computer from the
[Singular home page](https://www.singular.uni-kl.de).
In addition, if you have installed Sage on your computer,
you can access Singular from within Sage.
(The Sage installation includes a full installation of Singular.)

### Polynomials

All the basic operations with polynomials can be done in Singular.
I will try to add directions later.


### Polynomial division

Unfortunately the default division algorithm in Singular is slightly different
from the simplified algorithm presented in the textbook.
Here is a Singular implementation of the exact division algorithm from the textbook
(adapted from code by Greg Smith).

```
proc ivadivision ( poly f, list G)
{
  poly p = f;
  poly r = 0*f;
  int m = size(G);
  int i;
  list Q;
  for (i=1; i <= m; i++ ) { Q[i] = 0*f; }
  
  while (p != 0)
  {
    // Find first i such that lead(p) is divisible by lead(G[i])
    for (i=1; i <= m; i++)
    {
      if( (lead(p) / lead(G[i])) * lead(G[i]) == lead(p) )
      {
        break;
      }
    }
    
    if ( i <= m )
    {
      Q[i] = Q[i] + (lead(p) / lead(G[i]));
      p = p - (lead(p) / lead(G[i]))*(G[i]);
    } else {
      r = r + lead(p);
      p = p - lead(p);
    }
  }
  
  list ret = (r,Q);
  return(ret);
}
```

(Observe that the syntax is largely C-like, but arrays are indexed starting from 1.)
