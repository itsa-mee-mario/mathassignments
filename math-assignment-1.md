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
