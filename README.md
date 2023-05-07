Download Link: https://assignmentchef.com/product/solved-eml5311-control-systems-theory-mechanical-and-aerospace-engineering-hw-5
<br>
<em>You are encouraged to use MATLAB</em><sup> c </sup><em>to verify your answers whenever you can. However, unless specified, do not use MATLAB</em><sup> c </sup><em>to solve a problem.</em>

<strong>Problem 1. </strong>Let

<ol>

 <li>Determine the range space of the matrix <em>A </em>above and show it pictorially. (hint: you should be able to determine the linearly independent columns by inspection. If you cannot, reduce it to row-echelon form)</li>

 <li>What is the rank of this matrix? Verify your answer by using the rank command in MATLAB<sup> c </sup>.</li>

 <li>Determine the null space of the matrix <em>A </em>above show it pictorially.</li>

</ol>

<strong>Problem 2.             </strong>1. Find a basis for R(<em>A</em>), where  . (hint: you should be able to

do this by inspection). Show R(<em>A</em>) pictorially.

<ol start="2">

 <li>What is the rank of this matrix? Verify your answer by using the rank command in MATLAB<sup> c </sup>.</li>

 <li>Compute an orthonormal basis of R(<em>A</em>) for the <em>A </em>given in part 1 by using the orth command in MATLAB<sup> c </sup>. Show the span of this basis pictorially. (The MATLAB<sup> c </sup>answer may look different from your answer at first glance, but the picture will tell you they are the same)</li>

</ol>

<strong>Problem 3.            </strong>1. Compute a row-echelon form of the following matrix:

(1)

<ol start="2">

 <li>What is the R(<em>A</em>)? (write it as the span of basic columns of <em>A</em>)</li>

 <li>Determine the null space, N(<em>A</em>) (write it as the span of a basis of the null space)</li>

 <li>What is the rank of <em>A</em>?</li>

</ol>

<strong>Problem 4. </strong>Consider the following system of linear equations:

<em>x</em><sub>1 </sub>+ 2<em>x</em><sub>2 </sub>+ <em>x</em><sub>3 </sub>= 2

2<em>x</em><sub>1 </sub>+ 4<em>x</em><sub>2 </sub>= 2 3<em>x</em><sub>1 </sub>+ 6<em>x</em><sub>2 </sub>+ <em>x</em><sub>3 </sub>= 4

<ol>

 <li>Does it have no solution, an unique solution, or infinite number of solutions?</li>

 <li>If no solutions, say so. If there is an infinite number of solutions, find one. If there is an unique solution, find that one.</li>

</ol>

<strong>Problem 5. </strong>Consider the system of linear equations <em>Ax </em>= <em>y</em>, where:

<ol>

 <li>Does it have no solution, an unique solution, or infinite number of solutions?</li>

 <li>If no solutions, say so. If there is an infinite number of solutions, find one. If there is an unique solution, find that one.</li>

</ol>

<strong>Problem 6. </strong>1. Compute the eigenvalues and eigenvectors of by hand, and then verify your answer by using the eig command in MATLAB<sup> c </sup>.

<ol start="2">

 <li>Is this matrix diagonalizable? (hint: compute the eigenvectors) <strong>Problem 7. </strong>Consider the matrix:</li>

</ol>

What is the rank of this matrix? 3, since it has exactly 3 non-zero eigenvalues.

Prove the following generalization of this observation: If a real symmetric <em>n </em>× <em>n </em>matrix <em>A </em>has <em>m </em>zero eigenvalues and <em>m &lt; n </em>(meaning, it has <em>n </em>− <em>m </em>non-zero eigenvalues), the rank of the matrix is <em>n </em>− <em>m</em>. (Hint: use diagonalization, and then use the following result: if <em>X,Y,Z </em>∈R<em><sup>n</sup></em><sup>×<em>n </em></sup>and <em>X,Z </em>are invertible, then the rank of the product matrix <em>XY Z </em>is equal to the rank of <em>Y </em>. )

<strong>Problem 8. </strong>Suppose <em>a </em>∈R<em><sup>n</sup></em>. Prove that the <em>n </em>× <em>n </em>matrix <em>aa<sup>T </sup></em>has only one non-zero eigenvalue, which is given by <em>a<sup>T</sup>a</em>. What is the corresponding eigenvector? ( Hint: That there is only one non-zero eigenvector follows from a rank argument that uses the result from the previous problem. Call that <em>λ</em>. if <em>v </em>is the corresponding eigenvector, then <em>Mv </em>= <em>λv</em>. Pre multiply both sides by <em>a<sup>T </sup></em>and recognize that <em>v<sup>T</sup>a </em>= <em>a<sup>T</sup>v </em>because <em>v<sup>T</sup>a </em>is a scalar so it is equal to its transpose. )

<strong>Problem 9. </strong>Consider the two square matrices <em>A </em>and <em>A</em>−<em>µI</em>, where <em>µ </em>is an arbitrary constant. Prove that

<ol>

 <li>if <em>λ </em>is an eigenvalue of <em>A</em>, then <em>λ </em>− <em>µ </em>is an eigenvalue of <em>A </em>− <em>µI</em>,</li>

 <li>The two matrices have the same set of eigenvectors.</li>

</ol>

<strong>Problem 10. </strong>[Similarity preserves eigenvalues] Two matrices <em>A </em>and <em>B </em>are called <em>similar </em>if there exists an invertible matrix <em>V </em>such that <em>V </em><sup>−<a href="#_ftn1" name="_ftnref1">[1]</a></sup><em>AV </em>= <em>B</em>. Prove that if two matrices are similar, they have the same set of eigenvalues<sup>1</sup>.

<strong>Problem 11 </strong>(A fun(?) exercise. There nothing to submit; will not be graded)<strong>. </strong>Run the following MATLAB<sup> c </sup>code segment to visualize the range space of the <em>A </em>matrix provided in the code.

clear all

A = [1 2; 2 -3; 3 5];

fh = figure allxs = randn(2,1000)*10; allys = A*allxs; figure(fh); hold on; plot3(allys(1,:),allys(2,:),allys(3,:),’b.’); plot3(0,0,0,’r*’); grid on; set(gca,’CameraPosition’, [316.5072 -1.7181e+03 1.4311e+03]); set(gca,’CameraTarget’, [-10 -11.8747 0]); set(gca,’CameraUpVector’,[0 0 1]); set(gca,’CameraViewAngle’,9.4228);

<a href="#_ftnref1" name="_ftn1">[1]</a> This result will be useful later to show that a transfer function can be realized by an infinite number of state space models