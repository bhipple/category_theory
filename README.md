###Category Theory for Scientists
Notes while reading the textbook at:  
http://math.mit.edu/~dspivak/teaching/sp13/CT4S--static.pdf  

####Brief Set of mappings to be explored later:  
Hierarchies -> Posets  
Symmetries -> Group elements  
Data models -> Categories  
Agent Actions -> Monoid actions  
Local-global principles -> Sheaves  
Self-similarity -> Operads  
Context -> Monads  

####Other References
Conceptual Mathematics, by Lawvere and Schanuel  
Categories for the working mathematician, by Mac Lane  
Category Theory for computing science, by Barr and Wells  

####The Category of Sets
Let X and Y be sets.  A function f:X-->Y is a mapping that sends each element x in X, the domain of f, to an element y in Y, the codomain of f.  

Given function f:X-->Y, the elements y in Y that have at least one x in X such that f(x) = y are said to be in the image of f.  

Two functions f:X-->Y and g:Y-->Z are asid to be composable if the codomain of f is the domain of g, which we denote as gof:X-->Z  

A function f:X-->Y is called an isomorphism if there exists a function g:Y-->X such that gof = identity_x and fog = identity_y.  We also say that f is invertible and we say that g is the inverse of f.  If there exists an isomorphism X-->Y, we say that X and Y are isomorphic sets.  

Lemma 2.1.2.10:  
1) Any set A is isomorphic to itself (reflexive)  
2) For any sets A and B, if A is isomorphic to B, then B is isomorphic to A (symmetric)  
3) For any sets A, B, and C, if A is isomorphic to B and B is isomorphic to C, then A is isomorphic to C (transitive)  

#####Exercise 2.1.1.2
Let A = {1,2,3}. Then the subsets of A are {}, {1}, {2}, {3}, {1,2}, {2,3}, {1,3}, {1,2,3}  

#####Exercise 2.1.2.2
There is a function maping PR cells to RG cells, since for all x in PR there exists f:PR-->PG.  However, because a PG cell may connect with many PR cells, there does not exist a well defined g:PG-->PR covering the full set of connections.  

#####Exercise 2.1.2.3
The image of the above set Y is {y1, y2, y4}

#####Exercise 2.1.2.4
Let A = {1,2,3,4,5} and B = {x,y}. The set off all Hom_set(X,Y) functions mapping X to Y contains 2^5 = 32 distinct functions.

#####Exercise 2.1.2.5
Any set A such that |A| = 1 has the property that there is only one function in Hom_set(B, A) for any B.

#####Exercise 2.1.2.9
Let X be a set with n elements, where n is in N.  There are n choose 2 isomorphisms from X to itself?  And when n = 0, it seems there are infinitely many functions, each of which is equivalent to all of the others; either that, or there are 0 functions.  TODO

#####Exercise 2.1.2.11
Let A = {a, 7, Q}, B = {Bob, Club, r8}.  Consider a set C={1,2,3,4,5} together with a function f:B-->C such that f(Bob)=1, f(Club)=3, and f(r8)=4.  Since A and B are isomorphic, there exists functions g:A-->B and g':B-->A.

The function fog:A-->C is the induced mapping from A to C.  

#####Exercise 2.1.2.12
Find a set A such that for any set X there iss an isomorphism of sets X ~= Hom_set(A,X).  TODO

#####Exercise 2.1.2.13
Let A = {a,b,c,d}.  If f:10-->A is given by (a,b,c,c,b,a,d,d,a,b), then f(4) = c.  

The sequence s is 1, 4, 9, 16, 25, 36, 49  

#####Exercise 2.1.2.15
If A = {5,6,7}, then |A| = 3.  |N| is countably infinite, while |{n in N | n <= 5}| = 6  
