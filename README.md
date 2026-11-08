# Consecutive Residues — OEIS A000445

**https://guillochon.github.io/consecutive-residues/**

[A000445](https://oeis.org/A000445) asks how late the first pair of consecutive n-th power residues can come,
over all primes: 9, 77, 1224, 7888, 202124, 1649375 for n = 2..7 (Lehmer, Lehmer, Mills, Dunton, Bierstedt,
Brillhart, 1962–1964). For 8th powers the value is **a(8) = 1508324**: the first pair is
1508324 = 2²·47·71·113 and 1508325 = 3·5²·7·13²·17. Don Reble had bounded it as 1499876 ≤ a(8) ≤ 1508324 in 2019.

The page has four figures:

- **The long run.** All numbers 1..a(k)+1 as a grid, residues dark, for the extremal character of each k (and the
  1964 vector for k = 8). A lens shows χ(n), the index of n mod k, and explains each value from n's factorization.
  The browser rebuilds the character from its values on primes and checks where the first pair lands.
- **The characters.** For each k, which primes get a value other than χ = 1 in a maximal choice.
- **Ordinary primes.** The first pair r(p) for every prime p ≡ 1 (mod k) up to 4·10⁶, computed in the browser,
  against a(k). For k = 8, no prime below 10⁶ gets past r = 510.
- **The impossibility proof.** Statistics of the checked proof tree showing no character avoids a pair below
  1508325: nodes per prime and the 1.2 million pairs that close its branches.

Everything runs in one file (`index.html`). The method, the certificate and the checkers are in
[oeis-results/A000445](https://github.com/guillochon/oeis-results/tree/main/A000445).

Made by James Guillochon with Claude. The source lives in the oeis-sniper project (`viz/A000445/`); this repo holds
the published copy.
