Download Link: https://assignmentchef.com/product/solved-prolog-assignment4-permutation-combination-and-sorting
<br>
<strong>Write Prolog programs for the following. </strong>

<ol>

 <li><strong>Remove the K’th element from a list.</strong> Example:</li>

</ol>

?- remove_at(X,[a,b,c,d],2,R).

{X = b, R = [a,c,d]}

<ol start="2">

 <li><strong>Extract a given number of randomly selected elements from a list.</strong></li>

</ol>

The selected items shall be put into a result list.

Example:

?- rnd_select([a,b,c,d,e,f,g,h],3,L).

{L = [e,d,a]}




Hint: Use the built-in random number generator random/2 and the result of problem P1.

<ol start="3">

 <li><strong>Generate a random permutation of the elements of a list.</strong></li>

</ol>

Example:

?- rnd_permu([a,b,c,d,e,f],L).

{L = [b,a,d,c,e,f]}




Hint: Use the solution of problem P2.

<ol start="4">

 <li><strong>Generate the combinations of K distinct objects chosen from the N elements of a list</strong></li>

</ol>

In how many ways can a committee of 3 be chosen from a group of 12 people? We all know that there are C(12,3) = 220 possibilities (C(N,K) denotes the well-known binomial coefficients). For pure mathematicians, this result may be great. But <em>we</em> want to really generate all the possibilities (via backtracking).







Example:

?- combination(3,[a,b,c,d,e,f],L).

{L = [a,b,c]} ;

{L = [a,b,d]} ;

{L = [a,b,e]} ;

…

<ol start="5">

 <li><strong>Sorting a list of lists according to length of sublists</strong>

  <ol>

   <li>We suppose that a list (InList) contains elements that are lists themselves. The objective is to sort the elements of InList according to their <strong>length</strong>. E.g. short lists first, longer lists later, or vice versa.</li>

  </ol></li>

</ol>




Example:

?- lsort([[a,b,c],[d,e],[f,g,h],[d,e],[i,j,k,l],[m,n],[o]],L).

{L = [[o], [d, e], [d, e], [m, n], [a, b, c], [f, g, h], [i, j, k, l]]}




<ol>

 <li>Again, we suppose that a list (InList) contains elements that are lists themselves. But this time the objective is to sort the elements of InList according to their <strong>length frequency</strong>; i.e. in the default, where sorting is done ascendingly, lists with rare lengths are placed first, others with a more frequent length come later.</li>

</ol>




Example:

?- lfsort([[a,b,c],[d,e],[f,g,h],[d,e],[i,j,k,l],[m,n],[o]],L).

{L = [[i, j, k, l], [o], [a, b, c], [f, g, h], [d, e], [d, e], [m, n]]}




Note that in the above example, the first two lists in the result L have length 4 and 1, both lengths appear just once. The third and forth list have length 3 which appears, there are two list of this length. And finally, the last three lists have length 2. This is the most frequent length.

<ol start="6">

 <li><strong>Implement Permutation Sort. </strong></li>

 <li><strong>Implement Bubble Sort. </strong></li>

 <li><strong>Implement Selection Sort. </strong></li>

 <li><strong>Implement Insertion Sort. </strong></li>

 <li><strong>Implement Merge Sort. </strong></li>

 <li><strong>Implement Quick Sort using Accumulator. </strong></li>

 <li><strong>Implement Quick Sort without Accumulator. </strong></li>

</ol>

<strong> </strong>