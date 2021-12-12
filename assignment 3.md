1. if $$ y = \frac{x} {x^2 + a^2}$$ find $y_n$
denominator can be factorised as
$(x - ia)(x + ia)$,
using partial fractions method
$$y = \frac{A}{(x- ia)} + \frac B {(x+ib)} $$
where
$$A(x+ib) + B(x-ib) = x$$
$$x(A+B) +ib(A-B) = x$$ 
so, $A+B = 1$ and $A-B = 0$
then $A= 0.5,  B = 0.5$
$$y = \frac{1}{2(x- ia)} + \frac 1 {2(x+ib)}$$
$$y = 0.5 (\frac{1}{(x- ia)} + \frac 1 {(x+ib)})$$
taking the $n^{th}$ derivative
$$y_{n}= 0.5(-1)^{n}n! ((x-ia)^{-(n+1)} + {(x+ia)^{-(n+1)}})$$
put $x = rcos\theta$ and $a = rsin\theta$ (so that we can later use De Moivre's Theorem to cancel out the imaginary terms)
$$y_{n}= 0.5 -1^{n}n! [(rcos\theta - irsin\theta)^{-(n+1)} +(rcos\theta + irsin\theta)^{-(n+1)}]$$
taking out $r^{-(n+1)}$ 
$$y_{n}= -1^{n}n! \  r^{-(n+1)} (cos[(n+1)\theta] )$$
putting back the value of $r$ in terms of $\theta$
$$r^{(n+1)} = a^{n+1} sin^{(n+1)} \theta$$
$$y_{n}= -1^{n}n! \  (a^{n+1} sin^{(n+1)} \theta )^{-1} (cos[(n+1)\theta] )$$
$$y_{n}=\frac{-1^{n}n! sin^{(n+1)}\phi cos(n+1)\phi } {a^{n+1}}$$
where $\phi = tan^{-1}(x/a)$ 


---
2. $$y = e^{x}sin^{2}x$$

$$y = \frac 1 2 e^{x} (1- cos2x)$$

$$y = \frac{e^{x}}{2} - \frac{e^{x}cos2x}{2}$$

$$y_{n}=  \frac{x^{n}e^{x}}{2} - \frac{e^{x}\sqrt{3}^{n}cos(2x+ ntan^{-1} 2)}{2}

$$
      


---

3. $$y = log((ax+b) (cx+d))$$
	$$y = log(ax+b) + log(cx+d)$$
	$$y_{n}= \frac{(-1)^{n-1}a^{n} (n-1)! }{{(ax+b)}^{n}} + \frac{-1^{n-1}c^{n}(n-1)!}{(cx+d)^n}$$
	
---

4. x$$y = \begin{bmatrix} x+ \sqrt{(1+x^{2})}  \end{bmatrix} ^{m}   $$
differentiating wrt x:
$$y_{1}= m[x+ (1+x^{2})^{\frac{1}{2}}][1 + (1+x^{2})^{\frac{-1}{2}}(x)]$$
$$y_{1}= m[x+ (1+x^{2})^{\frac{-1}{2} }x^{2} +(1+x^{2})^{\frac{1}{2}} + x]$$
$$y_{1}= m\left[2x (1+x^{2})^{\frac{1}{2} }+(1+2x^{2}) \right](1+x^{2})^{\frac{-1}{2} }$$

$$
(1+x^{2})^{\frac{1}{2}} y_{1}= m\left[2x(1+x^{2})^{\frac{1}{2}} + 1+2x^{2}\right]
$$

squaring both sides:
$$
(1+x^{2}) y_{1}^{2} = m^{2} \left[2xy^\frac{1}{m}+1\right]^2
$$

differentiating again:
$$
y_{1}^{2}2x + 2(1+x^{2})y_{1}y_{2}= 2m^{2} \left[2xy^\frac{1}{m}+1\right]\left[2y^{\frac{1}{m}}+2x\frac{y^{(\frac{1}{m}-1)}}{m}y_{1}\right]
$$


---

5

---
6. if $y = cos(m sin^{-1}x )$ show that $(1-x^{2})y_{n+2} -(2n + 1)x y_{n+1}-(n^{2}- m^{2})y_{n}= 0$

$$y_{1}= -sin(m sin^{-1}x ) m \frac {1} { \sqrt{(1-x^2)}} $$

squaring both sides:
$$y_{1}^{2} = m^{2}sin^{2}\frac{msin^{-1}x}{(1-x^{2})}$$

$$(1-x^{2})y_{1}^{2} = m^{2}sin^{2}({msin^{-1}x})$$

$$(1-x^{2})y_{1}^{2} = m^{2}(1- cos^{2}({msin^{-1}x}))$$

$$(1-x^{2})y_{1}^{2} = m^{2}(1- y^{2})$$

differentiating again
$$2y_{1}y_{2}- 2xy_{1}- 2x^{2}y_{2}y_{1} = m^{2}(-2y y_1)$$


dividing by $2y_{1}$ 
$$y_{2}- x- x^{2}y_{2} = m^{2}(-2y y_1)$$

---

7. from 
	$$e^{x}= 1+ x + \frac{x^{2}}{2!} + \frac{x^{3}}{3!}+ \frac{x^{4}}{4!}+...$$
	
	we find
	
	$$e^{-x}= 1- x + \frac{x^{2}}{2!} - \frac{x^{3}}{3!}+ \frac{x^{4}}{4!}+...$$
	
	giving us:
	$$xe^{-x}= x- x^2 + \frac{x^{3}}{2!} - \frac{x^{4}}{3!}+ \frac{x^{5}}{4!}+...$$
	
	which is the taylor series expansion of $xe^-x$
	
	
	---
	 
8. maclaurin series :

$$
f(x) = f(0) + f'(0)x + \frac{f''(0)x^{2}}{2!} +...
$$

$$
f(x) = \frac{x}{1+x^{2}}
, f(0) = 0
$$

$$f'(x) = -\frac{x^2-1}{(x^{2}+1)^{2}}$$ 
$$f'(0) = -1$$


$$f''(x) = 2x\frac{x^{2}-3}{(x^{2}+1)^{3}}$$
$$f''(0) = 0$$

$$
f'''(0)= -6
$$
 
using this info, the expansion till three terms is:
$$x-x^{3}+x^{5}$$

---

9. $$f(x) = f(0)+ f'(0)x + \frac{f''(0)x^{2}}{2!} + ...$$

$$f(x) = cos(sin(x))$$
$$f(0) = 1$$
$$f'(x) = -cos(x)sin(sin(x))- cos^2(x)cos(sin(x))$$
$$f'(0) = 0$$
$$f''(x)= sin(x)sin(sin(x))- cos^{2}(x)cos(sin(x))$$
$$f''(0)= -1$$
$$f'''(0)= 5$$

thus, the first three terms are $1 - \frac{x^{2}}{2}+ \frac{5x^{4}}{24}$

---

10. $$f(x) = f(0)+ f'(0)x + \frac{f''(0)x^{2}}{2!} + ...$$

$$f(x) = sin(sin(x))$$

$$f(0) = 0$$

$$f'(x) = cos(x)cos(sin(x))$$

$$f'(0) = 1$$

$$f''(x) = -sin(x)cos(sin(x)) - cos^2(x)sin(sin(x))$$

$$f'''(0)= -2$$

$$f'''''(0)= 12$$

thus the first three terms of the expansion is 
$x - \frac{x^{3}}{3}+ \frac{x^{5}}{10}$

---


11.
$$f(x)= f(a)+ f'(a)(x-a)+ \frac{f''(a)(x-a)^{2}}{2!}+...$$

$$f(x)=sin(\pi x)$$

$$f'(x)=\pi cos(\pi x)$$

$$f'(a) = 0$$

$$f''(x)= -\pi^{2}sin(\pi x)$$

$$f''(a) = -\pi^{2}$$

so the expansion of 
$$1 - \frac{pi^{2}(x-0.5)^{2}}{2}+ \pi^{4} \frac{(x-0.5)^{4}}{24}$$

 the value is 0.9511


