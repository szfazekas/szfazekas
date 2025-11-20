# Distinct squares, runs, and other repetitions

___

The most basic repetitive structure is $xx$ called a square due to its form $xx = x^2$. A string is square-free if it contains no squares. It was shown by Thue [22,23] that there exist square-free and cube-free strings of infinite length over ternary, respectively, binary, alphabets. A string of length $n$ can have $\Theta(n^2)$ occurrences of squares (take the trivial example of a unary word), and it is known that the maximum number of primitively rooted square is $\Theta(n \log n)$ [6]. 

In [10], Fraenkel and Simpson proved that the maximum number of distinct squares in a word is bounded by twice the length of the word. They also conjectured the following,

> The number of distinct squares in a length n word is less than n.

In the same paper, there is a construction for a lower bound of $n − O(\sqrt{n})$. 
Another simple lower bound construction of the same order is binary words with k occurrences of b’s and with increasing number of a’s between each pair of consecutive b's. A number of alternative proofs of the 2n upper bound are known, see, e.g., [14] or [12]. The upper
bound was first improved to $2n − \Theta(\log n)$ in [15] and then to $11n/6$ in [8] by restricting the number of double squares (positions where the rightmost occurrences of two squares start). 

For larger exponents $k$, the number of distinct powers is less than $n/(k−2)$. For cubes the bound was improved to $4n/5$ in [5]. The problem involving higher exponents has its
inspiration in the investigation of the maximum number of runs in a string. Runs are maximal repetitions whose period is less than half of their length. The bound on their number was long conjectured to be less than the string's length [18], and recently proved to be as conjectured [1].

> The number of runs in a length n word is less than n.

This bound was improved to $≈ 0.9482n$ in [13], indicating that the optimal upper bounds will probably differ in the cases of runs and distinct squares.

Fraenkel and Simpson's conjecture was proved in 2023 by Shuo Li and Srečko Brlek [21].

## Our work

### Higher exponents and square networks
Prior to Brlek and Li's papers, we provided the best upper bounds on the [number of distinct repetitions of different exponents](https://www.worldscientific.com/doi/10.1142/S0129054110007416). 
We also introduced a graph theoretic approach to attack the problem of counting distinct squares by looking at the [networks induced by their shared special positions](https://www.sciencedirect.com/science/article/pii/S030439752100462X).

![image](/topics/fig/squares1.jpg)


### Clusters of repetition roots
We started the study of [clusters of repetition roots](https://link.springer.com/chapter/10.1007/978-3-030-67731-2_29), which are the set of positions in a string where said roots occur. We formulated a stronger conjecture than Fraenkel and Simpson’s, in terms of the lower bounds on the size of the clusters in terms of the number of clusters included in them. We proved [special cases of our conjecture](https://link.springer.com/chapter/10.1007/978-3-031-13257-5_4) when the nested clusters form a linear order. Following the proof by Brlek and Li of the Fraenkel-Simpson conjecture, we have been working extending their technique to give a full proof of our stronger conjecture, using the so called Rauzy graphs of the strings.

![image](/topics/fig/clusterEx2.png) &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp; <img src="/topics/fig/goals_old.png" alt="Goals" width="400"/>




The notebook on [cluster of repetitions](https://github.com/szfazekas/Combinatorics-on-Words/blob/master/clusters.ipynb) implements helper functions and some ideas presented in our paper with Robert Mercas from SOFSEM 2021. The notebook is not a finished product, so use with caution.
___
This work has been supported by JSPS KAKENHI Grant Number JP19K11815.
___

Publications on the topic:
- Szilárd Zsolt Fazekas, Robert Mercas: Clusters of Repetition Roots Forming Prefix Chains. DCFS 2022: 43-56
- Szilárd Zsolt Fazekas, Shinnosuke Seki: Square network on a word. Theor. Comput. Sci. 894: 121-134 (2021)
- Szilárd Zsolt Fazekas, Robert Mercas: Clusters of Repetition Roots: Single Chains. SOFSEM 2021: 400-409
- Maxime Crochemore, Szilárd Zsolt Fazekas, Costas S. Iliopoulos, Inuka Jayasekera: Number of Occurrences of powers in Strings. Int. J. Found. Comput. Sci. 21(4): 535-547 (2010)


Some related references:

1. Bannai, H.I.T., Inenaga, S., Nakashima, Y., Takeda, M., Tsuruta, K.: The “runs”
theorem. SIAM J. Comput. 46(5), 1501–1514 (2017)

2. Blanchet-Sadri, F., Merca ̧s, R., Scott, G.: Counting distinct squares in partial
words. Acta Cybern. 19(2), 465–477 (2009)

3. Blanchet-Sadri, F., Merca ̧s, R., Scott, G.: A generalization of Thue freeness for
partial words. Theor. Comput. Sci. 410(8–10), 793–800 (2009)

4. Crochemore, M., Fazekas, S., Iliopoulos, C., Jayasekera, I.: Number of occurrences
of powers in strings. Int. J. Found. Comput. Sci. 21(4), 535–547 (2010)

5. Crochemore, M., Iliopoulos, C., Kubica, M., Radoszewski, J., Rytter, W., Wale ́n,
T.: The maximal number of cubic runs in a word. J. Comput. System Sci. 78(6),
1828–1836 (2012)

6. Crochemore, M., Rytter, W.: Squares, cubes, and time-space efficient string search-
ing. Algorithmica 13(5), 405–425 (1995)

7. Dekking, F.: On repetitions of blocks in binary sequences. J. Combin. Theory Ser.
A 20, 292–299 (1976)

8. Deza, A., Franek, F., Thierry, A.: How many double squares can a string contain?
Discrete Appl. Math. 180, 52–69 (2015)

9. Fraenkel, A., Simpson, J.: How many squares must a binary sequence contain?
Electron. J. Combin. 2, #R2 (1995)

10. Fraenkel, A., Simpson, J.: How many squares can a string contain? J. Combin.
Theory Ser. A 82(1), 112–120 (1998)

11. Gusfield, D.: Algorithms on Strings, Trees, and Sequences - Computer Science and
Computational Biology. Cambridge University Press, Cambridge (1997)

12. Hickerson, D.: Less than 2n distinct squares in a word of length n, communicated
by Dan Gusfield (2003)

13. Holub, S.: Prefix frequency of lost positions. Theoretical Comput. Sci. ˇ 684, 43–52
(2017)

14. Ilie, L.: A simple proof that a word of length n has at most 2n distinct squares. J.
Combin. Theory Ser. A 112(1), 163–164 (2005)

15. Ilie, L.: A note on the number of squares in a word. Theoret. Comput. Sci. 380(3),
373–376 (2007)

16. Jonoska, N., Manea, F., Seki, S.: A stronger square conjecture on binary words. In:
Geffert, V., Preneel, B., Rovan, B., Stuller, J., Tjoa, A.M. (eds.) SOFSEM 2014. ˇ
LNCS, vol. 8327, pp. 339–350. Springer, Cham (2014). https://doi.org/10.1007/
978-3-319-04298-5 30

17. Kociumaka, T., Radoszewski, J., Rytter, W., Wale ́n, T.: Maximum number of
distinct and nonequivalent nonstandard squares in a word. Theor. Comput. Sci.
648(C), 84–95, October 2016

18. Kolpakov, R., Kucherov, G.: Finding maximal repetitions in a word in linear time.
In: Proceedings 40th FOCS, pp. 596–604. IEEE Computer Society Press (1999)

19. Lothaire, M.: Combinatorics on Words. Cambridge University Press, Cambridge
(1997)

20. Rampersad, N., Shallit, J., Wang, M.W.: Avoiding large squares in infinite binary
words. Theor. Comput. Sci. 339(1), 19–34 (2005)

21. Brlek, S., Li, S.: On the number of squares in a finite word. https://doi.org/10.48550/arXiv.2204.10204
___
[Back to main page](https://github.com/szfazekas/szfazekas)
