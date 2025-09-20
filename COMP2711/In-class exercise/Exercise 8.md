## Questions

Prove the following identity by combinatorial proof.

$$\sum_{k=1}^n k {n \choose k} = n2^{n-1}$$

$$\sum_{k=1}^n k {n \choose k} = \sum_{k=1}^n {k \choose 1} {n \choose k}$$

Suppose $n$ be the number of students in the course.  
$k$ be the number of the student(s) who get grade $A$.

${k \choose 1}$ means there is only one getting $A+$ in students who got A.

First item in left hand side, we have one A+ students among all k students in n students.  
Second item in left hand side, we have one A+ students and $1$ A students among all k students in n students.  
For the K item in LHS, we have one A+ students and $k-1$ A students among all k students in n students.

Alternatively, in all choices, we have $n$ A+ students, then we leave in total $2^{n-1}$ choices for choosing A students by using power set, since we have only n-1 students for A grade.

Therefore, $\sum_{k=1}^n k {n \choose k} = n2^{n-1}$.
