## Squares conjecture
___

The most basic repetitive structure is xx, where x is a non-empty string. Such
a string is also called, due to its form xx = x2, a square.
A string is said to be square-free or repetition-free if it contains no squares. It
was shown by Thue [22,23] that there exist square-free, respectively, cube-free,
strings of infinite length over a ternary, respectively, binary, alphabet. On the
other hand, it has been shown that the minimal number of distinct squares that
any sufficiently long binary string must contain is three [9].
A string of length n can have Θ(n2) occurrences of squares, by the trivial example of a unary word, and it is known that the maximum number of square occurrences xx, where x itself is not a repetition is Θ(n log n) [6]. Repetition counting
has also been investigated in other settings: when the length of the root (x for a repetition x) has length as small or large as possible (e.g., [7,9,20]), for partial words,
where words contain extra joker symbols that match every letter of the alphabet
(e.g., [2,3], as well as for abelian and other types of repetitions where the consecutive factors are not identical copies but equivalent in a looser sense (e.g. [17]).
Some, quite old and well studied, problems regarding this topic refer to the
maximal number of distinct repetitions that a word can have, as well as to the
maximum number of maximal repetitions (runs) that a string can contain.
This Work Was Supported By JSPS KAKENHI Grant Number JP19K11815.
c Springer Nature Switzerland AG 2021
T. Bureˇs et al. (Eds.): SOFSEM 2021, LNCS 12607, pp. 1–10, 2021.
https://doi.org/10.1007/978-3-030-67731-2_29
Author Proof
2 S. Z. Fazekas and R. Merca¸s
Problems. In [10], the authors prove that the maximum number of distinct
squares in a word is bounded by twice the length of the word (by looking at the
start position of the last occurrence of each square) and conjecture the following:
Conjecture 1. The number of distinct squares in a length n word is less than n.
In the same paper, the authors also provide a construction for a lower bound
of n − O(
√n). Another simple construction of a good lower bound of the same
order was provided in [16], by binary words with k occurrences of b’s and with
a number of a’s quadratic in k, which have 2k−1
2k+2n many distinct squares.
Several alternative proofs regarding the 2n upper bound are known, either
using combinatorics on words techniques [14], or just calculus [12]. The upper
bound was later improved to 2n − Θ(log n) in [15] by showing that the number
of double squares is bounded. Finally, in [8] the bound was reduced to 11n/6 by
using quite technical arguments to further restrict the number of double squares.
Regarding larger exponents, in [4] the authors showed that for a fixed integer
 > 2, the number of distinct -powers in a length n word is less than n
−2 . For
cubes, i.e.,  = 3 the bound was improved to 4n/5 in [5].
The latter problem involving repetitions of a higher fixed exponent, has its
inspiration in the investigation of the maximum number of runs that a word
can have. A run represents a repetition whose period is less than half and which
cannot be extended to either left or right in the given word, without breaking
the periodicity. The bound on this number was long conjectured to be less than
the word’s length [18], but only recently it is was showed to be the case [1].
Theorem 1. The number of runs in a length n word is less than n.
This bound was improved by Holub [13] to ≈ 0.9482n, indicating that the
optimal upper bounds will differ in the cases of runs and distinct squares.

___
Some related references:

1. Bannai, H.I.T., Inenaga, S., Nakashima, Y., Takeda, M., Tsuruta, K.: The “runs”
theorem. SIAM J. Comput. 46(5), 1501–1514 (2017)

1. Blanchet-Sadri, F., Merca ̧s, R., Scott, G.: Counting distinct squares in partial
words. Acta Cybern. 19(2), 465–477 (2009)

1. Blanchet-Sadri, F., Merca ̧s, R., Scott, G.: A generalization of Thue freeness for
partial words. Theor. Comput. Sci. 410(8–10), 793–800 (2009)

1. Crochemore, M., Fazekas, S., Iliopoulos, C., Jayasekera, I.: Number of occurrences
of powers in strings. Int. J. Found. Comput. Sci. 21(4), 535–547 (2010)

1. Crochemore, M., Iliopoulos, C., Kubica, M., Radoszewski, J., Rytter, W., Wale ́n,
T.: The maximal number of cubic runs in a word. J. Comput. System Sci. 78(6),
1828–1836 (2012)

1. Crochemore, M., Rytter, W.: Squares, cubes, and time-space efficient string search-
ing. Algorithmica 13(5), 405–425 (1995)

1. Dekking, F.: On repetitions of blocks in binary sequences. J. Combin. Theory Ser.
A 20, 292–299 (1976)

1. Deza, A., Franek, F., Thierry, A.: How many double squares can a string contain?
Discrete Appl. Math. 180, 52–69 (2015)

1. Fraenkel, A., Simpson, J.: How many squares must a binary sequence contain?
Electron. J. Combin. 2, #R2 (1995)

1. Fraenkel, A., Simpson, J.: How many squares can a string contain? J. Combin.
Theory Ser. A 82(1), 112–120 (1998)

1. Gusfield, D.: Algorithms on Strings, Trees, and Sequences - Computer Science and
Computational Biology. Cambridge University Press, Cambridge (1997)

1. Hickerson, D.: Less than 2n distinct squares in a word of length n, communicated
by Dan Gusfield (2003)

1. Holub, S.: Prefix frequency of lost positions. Theoretical Comput. Sci. ˇ 684, 43–52
(2017)

1. Ilie, L.: A simple proof that a word of length n has at most 2n distinct squares. J.
Combin. Theory Ser. A 112(1), 163–164 (2005)

1. Ilie, L.: A note on the number of squares in a word. Theoret. Comput. Sci. 380(3),
373–376 (2007)

1. Jonoska, N., Manea, F., Seki, S.: A stronger square conjecture on binary words. In:
Geffert, V., Preneel, B., Rovan, B., Stuller, J., Tjoa, A.M. (eds.) SOFSEM 2014. ˇ
LNCS, vol. 8327, pp. 339–350. Springer, Cham (2014). https://doi.org/10.1007/
978-3-319-04298-5 30

1. Kociumaka, T., Radoszewski, J., Rytter, W., Wale ́n, T.: Maximum number of
distinct and nonequivalent nonstandard squares in a word. Theor. Comput. Sci.
648(C), 84–95, October 2016

1. Kolpakov, R., Kucherov, G.: Finding maximal repetitions in a word in linear time.
In: Proceedings 40th FOCS, pp. 596–604. IEEE Computer Society Press (1999)

1. Lothaire, M.: Combinatorics on Words. Cambridge University Press, Cambridge
(1997)

2. Rampersad, N., Shallit, J., Wang, M.W.: Avoiding large squares in infinite binary
words. Theor. Comput. Sci. 339(1), 19–34 (2005)


[Back to main page](https://github.com/szfazekas/szfazekas)
