1. Elementary operations are row and column operations on a matrix which allow:
	1. scaling of rows/ columns,
	2. addition of rows/ columns
	
 Example: let matrix A:
$$A = 
\begin{bmatrix} 
	a & b & c \\
	c & d & e\\
	e & f & g \\
	\end{bmatrix} 
$$
applying $R_1 \rightarrow R_1 + R_2$  
gives:
$$A = 
\begin{bmatrix} 
	a+c & b+d & c+e \\
	c & d & e\\
	e & f & g \\
	\end{bmatrix} $$


and applying $R_1 \rightarrow 2R_1$  on the original matrix gives:
$$ A = 
\begin{bmatrix} 
	2a & 2b & 2c \\
	c & d & e\\
	e & f & g \\
	\end{bmatrix} 
$$
---
2. The rank of matrix is defined as the no. of linearly independent rows or columns.

	$$A = \begin{bmatrix} 
	1 & 0 & 2\\ 
	2 & 0 & 4\\
	1 & 1 & 1 \\
	\end{bmatrix} $$ 
	is a $3\times3$ matrix with rank 2 as it has exactly 2 linearly independent rows (when reduced to the simplest form)
	
	---


3.	Given:  $$ A = \begin{bmatrix} 
	1 & 2 & 3\\ 
	2 & 4 & 5\\
	3 & 5 & 6 \\
	\end{bmatrix} 	$$
	
	Applying $R_3 \rightarrow R_3 - R_2$ and $R_2 \rightarrow R_2-R_1$
	
	$$A = \begin{bmatrix} 
	1 & 2 & 3\\ 
	1 & 2 & 2\\
	1 & 1 & 1 \\
	\end{bmatrix}
	
	$$
	
	Applying $R_1 \rightarrow R_1 - R_2$ and rearranging
	we get 
	$$A = \begin{bmatrix} 
	
	1 & 2 & 2\\
	1 & 1 & 1 \\
	0 & 0 & 1\\ 
	\end{bmatrix}
	
	$$
	
	
	Applying $R_1 \rightarrow R_1 - R_2$ and rearranging
	we get 
	$$A = \begin{bmatrix} 
	
	
	1 & 1 & 1 \\
	0 & 1 & 1\\
	0 & 0 & 1\\ 
	\end{bmatrix}
	
	$$
	which can be reduced to 
	$$A = \begin{bmatrix} 
	
	
	1 & 0 & 0 \\
	0 & 1 & 0\\
	0 & 0 & 1\\ 
	\end{bmatrix}
	
	$$
	Which has 3 linearly independent rows/ columns and so has rank 3.
	
	---
	
	4.  A matrix is said to be in normal form when it can be represented as 
	
$$
	A = \begin{bmatrix}	
	I_r & 0 
	\end{bmatrix} \, ,

	A = \begin{bmatrix}	
	I_r \\ 0 
	\end{bmatrix} \, ,

	A = \begin{bmatrix}	
	I_r & 0 \\
	0 & 0
	\end{bmatrix}\, ,
	
	A = \begin{bmatrix}	
	I_r 
	\end{bmatrix}
$$
Where $I_r$ is the identity matrix of order $r$ and $0$ is the null matrix of any order.
	
	A matrix $A$ is said to be in Echelon form when:
	1. Every row that has all entries 0 is below every row with non-zero entries
	2. First non zero entry is 1
	3. tuber of zeros before first non-zero entry of a row is greater than the previous row.
---
5. a.
Given matrix 
	$$
	A = \begin{bmatrix} 
	1 & 2 & 3 & 0 \\
	2 & 4 & 3&2\\
	3 & 2 & 1& 3\\
	6&8&7&5\\
	\end{bmatrix}
	$$
	Apply $R_3 \rightarrow R_3-(R_1+R_2)$ to get:
	$$
		A = \begin{bmatrix} 
	1 & 2 & 3 & 0 \\
	2 & 4 & 3&2\\
	3 & 2 & 1& 3\\
	0&0&0&0\\
	\end{bmatrix}$$
	Apply $R_2 \rightarrow R_2-2R_1$ and divide by $-3$ , and apply $C_2 \rightarrow C_2/2$ to get:
	$$
	A = \begin{bmatrix} 
	1 & 2 & 3 & 0 \\
	0 & 0 & 1& -\frac{2}{3}\\
	3 & 2 & 1& 3\\
	0&0&0&0\\
	\end{bmatrix}$$
	
	Apply $C_1 \rightarrow C_1 - C_2$ to get:
	
	$$A = \begin{bmatrix} 
	0 & 1 & 3 & 0 \\
	0 & 0 & 1& -\frac{2}{3}\\
	2 & 1 & 1& 3\\
	0&0&0&0\\
	\end{bmatrix}
	$$
	Simplifying further and rearranging, we get
		$$
		A = \begin{bmatrix} 
		1 & 1/2 & 1/2& 3/2\\
	0 & 1 & 3 & 0 \\
	0 & 0 & 1& -\frac{2}{3}\\
	
	0&0&0&0\\
	\end{bmatrix}
	$$
	
	Which is in Echelon form, and we can now see that the rank of given matrix is 3.
---
b. 
Given matrix 
$$
	A = \begin{bmatrix} 
	-1 & 1 & -1& 1\\
	1 & -1 & 2 & -1 \\
	3 & 1 & 0 & 1
	\end{bmatrix}
$$
in this matrix, columns 2 and 4 are identical.
$$
	A = \begin{bmatrix} 
	-1 & 1 & -1& 0\\
	1 & -1 & 2 & 0 \\
	3 & 1 & 0 & 0
	\end{bmatrix}$$
	
Apply $C_1\rightarrow C_1+C_2$ and $R_2\rightarrow R_2+R_3$
$$
A = \begin{bmatrix} 
	0 & 0 & -1& 0\\
	0 & 0& 2 & 0 \\
	4 & -1& -5 & 0
	\end{bmatrix}
$$
Apply $C_3\rightarrow C_3-(C_2-C_1)$ and divide $C_1$ by 4

$$
A = \begin{bmatrix} 
	0 & 0 & -1& 0\\
	0 & 0& 2 & 0 \\
	1 & -1& 1 & 0
	\end{bmatrix}
$$
Apply $C_1\rightarrow C_1+C_2$  and $R_2 \rightarrow R_2/2+R_1$, followed by $R_3\rightarrow R_3+R_1$
$$  
A = \begin{bmatrix} 
	0 & 0 & -1& 0\\
	0 & 0& 0 & 0 \\
	0 & -1& 0 & 0
	\end{bmatrix}
$$

There are 2 linearly independent rows and columns to the rank of the matrix is 2.

---
c.
$$  
A = \begin{bmatrix} 
	1 & 4 & 8\\
	2 & 10& 22  \\
	0 & 4& 12
	\end{bmatrix}
$$

Apply $R_2\rightarrow R_2/2$ and $R_2\rightarrow R_2-R_3$ to get

$$  
A = \begin{bmatrix} 
	1 & 4 & 8\\
	1 & 1& -1  \\
	0 & 4& 12
	\end{bmatrix}
$$
Apply $R_1\rightarrow R_1-R_3$
and $R_3\rightarrow R_3/4$
$$  
A = \begin{bmatrix} 
	1 & 0 & -4\\
	1 & 1& -1  \\
	0 & 1& 3
	\end{bmatrix}
$$

Apply $R_3\rightarrow R_3+(R_1-R_2)$

$$  
A = \begin{bmatrix} 
	1 & 0 & -4\\
	1 & 1& -1  \\
	0 & 0& 0
	\end{bmatrix}
$$
simplify to get
$$  
A = \begin{bmatrix} 
	1 & 1 & -1\\
	0 & 1& -4 \\
	0 & 0& 0
	\end{bmatrix}
$$
Which is a matrix in echelon form with rank 2.

---
6.  
a. 
$$  
A = \begin{bmatrix} 
	1 & 2 & 1&2\\
	1 & 3& 2&2 \\
	2&4&3&4\\
	3&7&4&6
	\end{bmatrix}
$$
apply $R_2\rightarrow R_2-R_1, \ R_3\rightarrow R_3-2R_1, \ R_4\rightarrow R_4 -(3R_1+R_2+R_3)$
$$
A = \begin{bmatrix} 
	1 & 2 & 1&2\\
	0 & 1& 1&0\\
	0&0&1&0\\
	0&0&-1&0
	\end{bmatrix}
$$
apply $R_4\rightarrow R_4+R_3$ and reduce and rearrange the last column
$$ 
A = \begin{bmatrix} 
	0&1 & 2 & 1\\
	0&0 & 1& 1\\
	0&0&0&1\\
	0&0&0&0
	\end{bmatrix}
$$
is a matrix in echelon form with rank 3.

---

b.  
$$
A = \begin{bmatrix} 
	1&2&3&2\\
	2&3&5&1\\
	1&3&4&5
	\end{bmatrix}
$$
apply $R_2\rightarrow R_2-2R_1 \ , R_3\rightarrow R_3-R_1$

$$
A = \begin{bmatrix} 
	1&2&3&2\\
	0&-1&-1&-3\\
	0&1&1&3
	\end{bmatrix}
$$

taking negative of second row, subtracting from third:

$$
A = \begin{bmatrix} 
	1&2&3&2\\
	0&1&1&3\\
	0&0&0&0
	\end{bmatrix}
$$

is a matrix in echelon form and the rank is 2

---

c. 
$$
A = \begin{bmatrix} 
	1&2&1\\
	-1&0&2\\
	2&1&3
	\end{bmatrix}
$$
apply $R_2\rightarrow R_2+R_1$
$$
A = \begin{bmatrix} 
	1&2&1\\
	0&2&3\\
	2&1&3
	\end{bmatrix}
$$

apply $R_3\rightarrow R_3-2R_1$
$$
A = \begin{bmatrix} 
	1&2&1\\
	0&2&3\\
	0&-3&1
	\end{bmatrix}
$$
make first no zero elements 1:
$$
A = \begin{bmatrix} 
	1&2&1\\
	0&1&3/2\\
	0&1&-1/3
	\end{bmatrix}
$$
apply $R_3 \rightarrow R_3-R_2$ and appropriately scale the last row
$$
A = \begin{bmatrix} 
	1&2&1\\
	0&1&3/2\\
	0&0&1 
	\end{bmatrix}
$$


is  a matrix in echelon form with rank 3

---

7.   find $\alpha$ s.t. rank of 
$$
	A = \begin{bmatrix} 
	1&2&1\\
	0&1&3/2\\
	0&1&-1/3
	\end{bmatrix}
$$
is 3

(done in notebook, copy from pdf later)

---
8. reduce to echelon form:
$$	
	A = \begin{bmatrix} 
	1&3&-1&2\\
	0&11&-5&3\\
	2&-5 &3&1\\
	4&1&1&5
	\end{bmatrix}
$$
apply $R_3\rightarrow R_3-2R_1$
$$	
	A = \begin{bmatrix} 
	1&3&-1&2\\
	0&11&-5&3\\
	0&-11&5&-3\\
	4&1&1&5
	\end{bmatrix}
$$
subtract row 1 from 2 and rearrange:

$$	
	A = \begin{bmatrix} 
	1&3&-1&2\\
	4&1&1&5\\
	0&11&-5&3\\
	0&0&0&0
	\end{bmatrix}
$$







is in echelon form and has rank 3

---
9.
$$	
	A = \begin{bmatrix} 
	1&2&-1&3\\
	4&1&2&1\\
	3&-1&1&2\\
	1&2&0&1
	\end{bmatrix}
$$
apply $R_2 \rightarrow R_2-4R1$ and $R_3 \rightarrow R_3 -3R_1$ and $R_4 \rightarrow R_4-R_1$
 
 
$$	
	A = \begin{bmatrix} 
	1&2&-1&3\\
	0&-7&6&-11\\
	0&-7&-2&-7\\
	0&0&1&-2
	\end{bmatrix}
$$
apply $R_3 \rightarrow R_3 - R_2$
$$	
	A = \begin{bmatrix} 
	1&2&-1&3\\
	0&-7&6&4\\
	0&0&-8&4\\
	0&0&1&-2
	\end{bmatrix}
$$
apply $C_4 \rightarrow C_4+2C_3$
$$	
	A = \begin{bmatrix} 
	1&2&-1&1\\
	0&-7&6&16\\
	0&0&-8&0\\
	0&0&1&0\\
	\end{bmatrix}
$$
which can be reduced to:
$$	
	A = \begin{bmatrix} 
	1&0&0&0\\
	0&1&0&0\\
	0&0&1&0\\
	0&0&0&0\\
	\end{bmatrix}
$$

is a matrix of rank 3 in normal form.

---

10. Consistent system of linear equations has one or more solutions, and an inconsistent system has no solution. 

	A linear equation of the form $AX=B$ is Non-Homogeneous if $B$ is not a 0 vector, and it is called Homogeneous if $B$  is a null vector.
	
	For unique solution:
	if  $\rho(A)= \rho([A|B]) = n = r$ The system has a unique solution.
	
	if $\rho(A)<\rho([A|B])$ the system is inconsistent or has no solutions.
	
	if $m<n$ then there will be infinite solutions.
	
	---
11. A  system of linear equations is called Homogeneous if all the elements of the matrix B are zero. A Homogeneous system of linear equations can have either infinite or trivial solution, so it is always consistent.
12. values of m, k for which the system is consistent 
$$
x+ y+ z = 3 /
x+ 2y+ mz = 5 /
x +2y +4z = k
$$

the Augmented matrix of the system:
$$
b = \begin{bmatrix} 
	1&1&1&3\\
	1&2&m&5\\
	1&2&4&k\\
	\end{bmatrix}
$$
reduce to echelon form:
apply $R_3 \rightarrow R_3 -R_2$  and $R_2 \rightarrow R_2-R_1$ and divide $R_3$ by $4-m$
$$ 
b = \begin{bmatrix} 
	1&1&1&3\\
	0&1&m-1&2\\
	0&0&1&(k-5) / (4-m)\\
	\end{bmatrix}
$$
swapping $C_3$ and $C_4$
$$ 
b = \begin{bmatrix} 
	1&1&3&1\\
	0&1&2&m-1\\
	0&0&(k-5) / (4-m)&1\\
	\end{bmatrix}
$$

so, for the system to be consistent, $$k =5 , m \ne 4$$

---
13. Show that the system of linear equations has infinite solutions.

$$ 
b = \begin{bmatrix} 
	2&2&-3&1\\
	4&4&1&2\\
	6&6&-1&3\\
	\end{bmatrix}
$$
apply $R_3 \rightarrow R_3 + 2R_2 - R_1$
$$ 
b = \begin{bmatrix} 
	2&2&-3&1\\
	4&4&1&2\\
	0&0&0&0\\
	\end{bmatrix}
$$
this system has infinitely many solutions.

14. $$ 
[A|b] = \begin{bmatrix} 
	2&3&-1&1\\
	3&-4&3&-1\\
	2&-1&2&-3\\
	3&1&-2&4
	\end{bmatrix}
$$

if rank of A is not equal to rank of augmented matrix, then the non-homogeneous system is inconsistent and has no solution.
$$ 
[A] = \begin{bmatrix} 
	2&3&-1\\
	3&-4&3\\
	2&-1&2\\
	3&1&-2
	\end{bmatrix}
$$
can be reduced to 
$$ 
[A] = \begin{bmatrix} 
	2&3&-1\\
	0&1&-9/17\\
	0&0&1\\
	0&0&0
	\end{bmatrix}
$$
so the system is inconsistent

---
15. $$ 
[A] = \begin{bmatrix} 
	1&2&-1\\
	3&-1&2\\
	2&-2&3\\
	1&-1&1
	\end{bmatrix}
$$

$$ 
[A|b] = \begin{bmatrix} 
	1&2&-1&3\\
	3&-1&2&1\\
	2&-2&3&2\\
	1&-1&1&-1
	\end{bmatrix}
$$
simplifying A:
$$ 
[A] = \begin{bmatrix} 
	1&0&0\\
	0&1&0\\
	0&0&1\\
	0&0&0
	\end{bmatrix}
$$
which is a matrix of rank 3.
$$ 
[A|b] = \begin{bmatrix} 
	1&2&-1&3\\
	0&-7&5&-8\\
	0&0&1&4\\
	0&0&0&0
	\end{bmatrix}
$$
which is a matrix of rank 3
so the system is consistent. 

$AX =b$
we can find the solution using the augmented matrix
$$ 
[A|b] = \begin{bmatrix} 
	1&2&-1&3\\
	0&-7&5&-8\\
	0&0&1&4\\
	0&0&0&0
	\end{bmatrix}
$$
$z = 4, x = -1, y = 4$

---
17.  $$ 
[A|b] = \begin{bmatrix} 
	1&1&1&6\\
	1&2&3&10\\
	1&2&\lambda&\mu
	\end{bmatrix}
$$

case of 1. no solution: a system of inconsistent linear equations has no solutions. A system of linear equations is inconsistent when rank of Coefficient is not equal to rank of Augmented matrix

$$ 
[A] = \begin{bmatrix} 
	1&1&1\\
	1&2&3\\
	1&2&\lambda
	\end{bmatrix}
$$

can be simplified to
$$ 
[A] = \begin{bmatrix} 
	1&1&1\\
	0&1&2\\
	0&0&\lambda -3
	\end{bmatrix}
$$

for the system to have no solutions, $\lambda$ needs to be equal to 3, and should not be equal to 10.

case of 2. infinite solutions: $\lambda = 2$ and $\mu = 10$
as these values make the third equation linearly dependent on the second one

case 3. unique solution: $\lambda \ne 3$, as to have a unique solution, the number of linearly independent equations (rank) needs to equal or greater than the number of variables (n)

---
18.  x

19. x

---

# Assignment 2
1. Eigenvalue:
	Roots of the characteristic Equation $$|A -\lambda I| = 0$$ are called the eigenvalues of matrix A.
	
	eg. 
	$$A = \begin{bmatrix}
	0&1&2\\
	1&0&2\\
	1&2&0
	\end{bmatrix}
	$$
	the characteristic equation of the matrix is
	$$|A-\lambda I| =det( \begin{bmatrix}
	0-\lambda&1&2\\
	1&0-\lambda&2\\
	1&2&0-\lambda
	\end{bmatrix} )
	$$
	$$	= (-\lambda)(\lambda^2 - 4) - 1(-\lambda-4)+ 1(2+2\lambda)$$
	$$= (\lambda^3-7\lambda-6)$$
	$$= (\lambda+1)(\lambda^2-\lambda-6)$$
	then the eigenvalues are:
	-1, -2, 3
	
2. Eigenvectors:
	the vectors $X$ satisfying $$(A-\lambda_i I)X = 0$$ for each of the  eigenvalues $\lambda_i$ is called an eigenvector. in the above example:
		$$ (A+1 I)X =0$$
		$$ (A+2 I)X =0$$
		$$ (A-3 I)X =0$$
		give the eigenvectors:
		$$ \begin{bmatrix}
	1&3&0\\
	0&0&0\\
	0&1&-1
	\end{bmatrix}
	\begin{bmatrix}
	x_1\\
	x_2\\
	x_3
	\end{bmatrix} =0$$
	
	$x_1 +3x_2=0$ and let $x_2 =x_3 = k$ 
	then, out vector is 
	$$
	\begin{bmatrix}
	-3\\
	1\\
	1
	\end{bmatrix} 
	$$
	for the second eigenvector:
	$$ \begin{bmatrix}
	1&-1&0\\
	1&2&2\\
	0&0&0
	\end{bmatrix}
	\begin{bmatrix}
	x_1\\
	x_2\\
	x_3
	\end{bmatrix} =0$$
	
	we get $x_1 = x_2= k$ and $3k +2x_3 = 0 \implies x_3 = -3k/2$
	so the matrix X is 	
	$$
	\begin{bmatrix}
	-2\\
	-2\\
	3
	\end{bmatrix} 
	$$
	
	
using the third eigenvalue :
$$ 
\begin{bmatrix}
	-1&1&0\\
	1&-3&2\\
	-1&0&1
	\end{bmatrix}
	\begin{bmatrix}
	x_1\\
	x_2\\
	x_3
	\end{bmatrix} =0
$$
	
we get the eigenvector 	
$$
	\begin{bmatrix}
	1\\
	1\\
	1
	\end{bmatrix} 
$$
	
---
	
3.
$$
A = \begin{bmatrix}
	8&-4\\
	2&2
	\end{bmatrix} 
	$$
Eigenvalues are the roots of characteristic equation:
$|A-\lambda I| =0$
$$
det(\begin{bmatrix}
	8-\lambda&-4\\
	2&2-\lambda
	\end{bmatrix}) = 0	
$$
$$
 (8-\lambda)(2-\lambda)+ 8= 0	
$$

$$
 = (6 -\lambda)(4 -\lambda)= 0
$$
so the eigenvalues are 6 and 4, and the eigenvectors are:


$$
\begin{bmatrix}
	2&-4\\
	2&-4
	\end{bmatrix} X = 0
	\implies X=\begin{bmatrix}
	1\\1
	\end{bmatrix}
$$

$$
\begin{bmatrix}
	4&-4\\
	2&-2
	\end{bmatrix} X = 0
	\implies X=\begin{bmatrix}
	1\\2
	\end{bmatrix}
$$

---

4. 
$$
A = 
\begin{bmatrix} 
 6&8\\ 
 8&-6 
\end{bmatrix}
$$
the characteristic equation is:
$|A-\lambda I| = 0$
$$
|A-\lambda I| = 
det(\begin{bmatrix} 
 6-\lambda&8\\ 
 8&-6 -\lambda
\end{bmatrix})
= (6-\lambda )(-6-\lambda) - (64) = 0
$$
$$
-100 + \lambda^2 = 0
$$
$$
\lambda = \pm 10
$$
so the eigenvalues are +10 and -10.
Eigenvectors are the vectors X, for all eigenvalues, such that
$$(A-\lambda I)X = 0$$
so, 
$$(A-10 I)X = 0,\ \  (A+10 I)X = 0 $$
$$(A-10I)X = 
\begin{bmatrix} 
 -4&8\\ 
 8&-16
\end{bmatrix}
\begin{bmatrix} 
x_1 \\
x_2
\end{bmatrix}
$$

$$
\implies -4x_1+8x_8 = 0, \ 8x_1 - 16x_2 = 0
$$
solving,
$$
X = \begin{bmatrix}1\\-2 \end{bmatrix}
$$

next, $$(A+10 I)X = 0$$
$$(A+10I)X = 
\begin{bmatrix} 
 16&8\\ 
 8&4
\end{bmatrix}
\begin{bmatrix} 
x_1 \\
x_2
\end{bmatrix}
$$
solving for X:
$$
X= \begin{bmatrix} 2\\1 \end{bmatrix}
$$

---

5. 
$$
A = \begin{bmatrix} 
1&1&1\\
1&2&1 \\
3&2&3
\end{bmatrix}
$$
for eigenvalues:
$$
|A-\lambda I| = det(\begin{bmatrix} 
1-\lambda&1&1\\
1&2-\lambda&1 \\
3&2&3-\lambda
\end{bmatrix})
$$

$$
(1-\lambda)[(3-\lambda)(2-\lambda) - 2] - 1[(3-\lambda)-2] + 3[1-(2-\lambda)]
$$
for getting eigenvalues:

$$

-\lambda(\lambda - 1)(\lambda-5) = 0
$$

The eigenvalues are 0, 1, 5

Finding the eigenvectors:
$$
(A-\lambda I)X = 0
$$

$$
\begin{bmatrix} 
1&0&1\\
0&1&0 \\
1&0&1
\end{bmatrix} 
\begin{bmatrix} 
x_1\\x_2\\x_3
\end{bmatrix} =0
$$

$$x_1 = -x_3 = k,\ x_2=0$$

then the first eigenvector is:
$$\begin{bmatrix} 
1\\0\\-1
\end{bmatrix}$$

the second eigenvector:

$$
\begin{bmatrix} 
0&1&1\\
1&0&0 \\
0&0&0
\end{bmatrix} 
\begin{bmatrix} 
x_1\\x_2\\x_3
\end{bmatrix} =0
$$
so the next eigenvector is 
$$X = \begin{bmatrix}0\\-1\\1\end{bmatrix}$$

then, 
$$
 \begin{bmatrix} 
-5&4&0\\
-4&-1&1 \\
0&0&0
\end{bmatrix}
\begin{bmatrix} 
x_1\\x_2\\x_3
\end{bmatrix} = 0

$$
put $x_1 = 4k$ and $x_2 = 5k$:
$$x_3 = 16k-5k = 11k$$
hence, the required eigenvector is:
$$
\begin{bmatrix} 
4\\5\\11
\end{bmatrix} 
$$
---

6.
$$
A = \begin{bmatrix} 
1&1&3\\
1&5&1 \\
3&1&1
\end{bmatrix}
$$
the eigenvalues satisfy:
$$|A-\lambda I| = 0$$
$$
det(\begin{bmatrix} 
1-\lambda&1&3\\
1&5-\lambda&1 \\
3&1&1-\lambda
\end{bmatrix}
)=0
$$

$$
(\lambda+2)(\lambda - 3)(\lambda- 6) = 0
$$

so the eigenvalues are -2, 3, 6

finding the first eigenvector:
$$
\begin{bmatrix} 
1&0&1\\
0&1&0 \\
0&0&0
\end{bmatrix}X = 0
$$
the first eigenvector is 
$$\begin{bmatrix} 1\\0\\-1 \end{bmatrix}$$

the next eigenvector is 
$$
\begin{bmatrix} 
-2&1&3\\
0&0&0 \\
3&1&-2
\end{bmatrix}X = 0
$$

$$
X = \begin{bmatrix} 1\\-1\\1 \end{bmatrix}
$$

and the last eigenvector is:

$$
\begin{bmatrix} 
-5&1&3\\
0&0&0 \\
3&1&-5
\end{bmatrix}X = 0
$$

$$
X = \begin{bmatrix} 1\\2\\1 \end{bmatrix}
$$

---



7. $$
	A = 
	\begin{bmatrix} 
	-2&2&-3\\
	2&1&-6\\
	-1&-2&0
   	\end{bmatrix}
   $$
   
  the characteristic equation is:
  $$det(	\begin{bmatrix} 
	-2-\lambda&2&-3\\
	2&1-\lambda&-6\\
	-1&-2&0-\lambda
   	\end{bmatrix}) = 0
	
$$

the eigenvalues are 5, -3 and -3

finding the eigenvectors:

$$
	\begin{bmatrix} 
	-7&2&-3\\
	2&-4&-6\\
	-1&-2&-5
   	\end{bmatrix}X = 0
	
$$
gives us 
$$
X = \begin{bmatrix} 
1\\ 2\\ -1
\end{bmatrix}
$$

next, 

  $$	\begin{bmatrix} 
	1&2&-3\\
	0&0&0\\
	0&0&0
   	\end{bmatrix}X = 0
	
$$
gives:
$$X = \begin{bmatrix}1\\1\\1 \end{bmatrix}$$ twice, as the last two eigenvalues are the same


---
8. Cayley-Hamilton Theorem: 
 
Every square matrix satisfies the matrix analogue of its characteristic polynomial


Let $A$ be an $n\times n$ square matrix. the characteristic polynomial is:
$$|A-\lambda I| = (-1)^n(\lambda^n+ a_1\lambda^{n-1} + ... +a_n)$$
then the matrix equation

$$ X^n+ a_1X^{n-1} + ... +a_nI_n = O$$
is satisfied by $X=A$


---

9. 
$$
A = 
\begin{bmatrix}
1&1&1\\
1&2&1\\
3&2&3
\end{bmatrix}
$$ 

characteristic equation of the matrix:
$$
det(\begin{bmatrix}
1-t&1&1\\
1&2-t&1\\
3&2&3-t
\end{bmatrix}) = 0
$$

$$(1-t)[(3-t)(2-t) - 2] - (1)[(3-t)-2]+3[1-(2-t)] =0$$
$$(1-t)(4-5t+t^2)+4(t-1)=0$$
$$5t-6t^2+t^3=0$$

Cayley Hamilton Theorem is verified if the matrix A satisfies the matrix analogue of the characteristic equation

$$5A-6A^2+A^3=0$$

$$A^2 = \begin{bmatrix}
1&1&1\\
1&2&1\\
3&2&3
\end{bmatrix}

\begin{bmatrix}
1&1&1\\
1&2&1\\
3&2&3
\end{bmatrix}

= \begin{bmatrix}
5&5&5\\
6&7&6\\
14&13&14
\end{bmatrix}$$

$$
6A^2=
\begin{bmatrix}
30&30&30\\
36&42&36\\
84&78&84 
\end{bmatrix}
$$


$$A^3 = \begin{bmatrix}
5&5&5\\
6&7&6\\
14&13&14
\end{bmatrix}
\begin{bmatrix}
1&1&1\\
1&2&1\\
3&2&3
\end{bmatrix}
= 
\begin{bmatrix}
25&25&25\\
31&32&31\\
69&68&69
\end{bmatrix}
$$ 

$$
5A = 
\begin{bmatrix}
5&5&5\\
5&10&5\\
15&10&15
\end{bmatrix}
$$

$$
5A+A^3 = 
\begin{bmatrix}
30&30&30\\
36&42&36\\
84&78&84
\end{bmatrix}
$$

$$
5A+A^3-6A^2= O_{3\times 3}
$$
which verifies Cayley-Hamilton Theorem

---

10. X $$ A=\begin{bmatrix} 1&1&3\\ 1&3&-3\\ -2&-4&4 \end{bmatrix} $$
the characteristic equation of the matrix is

$$
det(\begin{bmatrix} 
1-t&1&3\\
1& 3-t&-3\\
-2& -4& 4-t
\end{bmatrix}) = 0
$$

$$
(1-t)[(4-t)(3-t)+ 12] -1[4-t+12] +(-2)[-3-3(3-t)]
$$

$$
(1-t)[24 -7t+ t^2 ] - [16-t]+[24- 6t]
$$

$$
32 -26t +8t^2- t^3  = 0
$$

Cayley Hamilton theorem states that the matrix analogue for this equation must be satisfied by A

$$32- 26A+ 8A^2 - A^3$$

$$A^2 = \begin{bmatrix} 
3&3&1\\
3& 1&-1\\
-4& -2& 6
\end{bmatrix} $$

$$
A^3 = \begin{bmatrix} 
2&2&0\\
2& 0&-2\\
-3& -1& 7
\end{bmatrix}
$$


---

11.
Similarity of matrices: Let A and B be square matrices of order n. Then, the matrix B is similar to A if there exists a non-singular matrix P such that $B=P^{-1}AP$

Diagonalization: A matrix A is said to be diagonalizable if it is similar to a diagonal matrix D. $D=P^{-1}AP$


---


12. 
$$ 
A = \begin{bmatrix} 
5&-1&5\\ 0&2&0\\ -5&3& -15
\end{bmatrix} 
$$

The characteristic equation of the matrix is:
$$|A-\lambda I| = 0 = det(\begin{bmatrix} 
5-\lambda&-1&5\\ 0&2-\lambda&0\\ -5&3& -15-\lambda
\end{bmatrix} )$$

$$
(5-\lambda)[(2-\lambda)(-15-\lambda) ]+ (-5)[-5(2-\lambda)] = 0
$$

$$
(5-\lambda)[ -30-13\lambda+ \lambda^2 ]+ [50-25\lambda)] = 0
$$

$$
 -100+70\lambda - 8\lambda^2 - \lambda^3  = 0$$


Matrix A satisfies the equation 
$$
-100+70A - 8A^2 - A^3  = 0
$$

for finding the inverse of the matrix, multiply the equation by $A^{-1}$

$$-100A^{-1}+70I - 8A - A^2  = 0$$

$$
+70I - 8A - A^2  = 100A^{-1}
$$

$$
+70I - 8A - A^2  =  \begin{bmatrix} 30& 0& 10 \\ 0&50&0\\ -10& 10& -10 \end{bmatrix}
$$

$$
A^{-1} = \frac{1}{100}\begin{bmatrix} 30& 0& 10 \\ 0&50&0\\ -10& 10& -10 \end{bmatrix}
$$

---

13. $$A = \begin{bmatrix} 1&2\\-1&3 \end{bmatrix} $$
find the value of 
$$$$

the characteristic equation is
$$det(\begin{bmatrix}1-\lambda  & 2 \\ -1 & 3-\lambda \end{bmatrix}) =0$$

$$5-4 \lambda + \lambda ^2 = 0$$
 Cayley Hamilton theorem will be verified if:
$$A^2-4A+5I = 0$$

dividing the required equation by the characteristic equation: 

$$( A^6 - A^5 - 2 A^4 - 6 A^3 - 14 A^2 - 31 A - 46) (A^2-4A+5I)
+ 231 - 31 A  $$

$$ 231 - 31 A= \begin{bmatrix}200 & 169 \\ 262 & 138\end{bmatrix}$$

---
