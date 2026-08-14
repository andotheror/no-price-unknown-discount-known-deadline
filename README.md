# No Price for an Unknown Discount at a Known Deadline

## Abstract

Discounted regret evaluates an online learner with exponentially larger weight on recent losses. If the discount factor is known, online gradient descent attains regret of order $DG/\sqrt{1-\lambda}$. A recent result adapts to an unknown discount factor over a continuum at an extra factor $\sqrt{\log T}$, using a logarithmic collection of experts and discounted meta-algorithms. We show that this adaptivity cost vanishes when the terminal horizon $T$ is known. One projected-gradient iterate with the increasing step sizes $\eta_t=D/(G\sqrt{2(T-t+1)})$, chosen without $\lambda$, satisfies simultaneously for every $\lambda\in[0,1]$

$$\mathrm{DReg}_T(\lambda)\le \sqrt2DG\sqrt{\frac{1-\lambda^T}{1-\lambda}},$$

where the ratio is $T$ at $\lambda=1$. For every fixed $\lambda$, even an algorithm told $\lambda$ has minimax expected regret at least $1/(4\sqrt2)$ of this upper bound. Thus a single discount-oblivious trajectory is pointwise minimax for the entire continuum, including effective horizons from one to $T$. The mechanism is a terminal-suffix principle. Increasing step sizes make every suffix ending at the known deadline regret-optimal. Abel summation expresses any exponential discount as a probability mixture of these suffixes, and Jensen's inequality produces the exact finite-horizon effective scale. The same argument applies to mirror descent and to every nonincreasing terminal weighting kernel. Besides closing the logarithmic gap, the result reduces the number of learner states and per-round updates from $O(\log T)$ to one.

## Contributions

Our main results are: (i) one discount-oblivious OGD trajectory with the exact uniform finite-horizon bound~, (ii) a pointwise minimax lower bound for every discount including both endpoints, (iii) a terminal-suffix mixture principle for arbitrary nonincreasing kernels, (iv) an online mirror-descent extension, and (v) a reduction from $O(\log T)$ expert states and meta-updates to one state and one projection per round. The deadline is essential to our construction. We separate this fixed-terminal objective from guarantees required at every unknown stopping time.

## Keywords

price, unknown, discount, known, deadline, discounted, regret, evaluates, online

## Files

- `main.pdf`
- `main.tex`
- `references.bib`
- `iclr2027_conference.sty`, `iclr2027_conference.bst`, `natbib.sty`, `fancyhdr.sty`
- `main.pdf.ots`, `README.md.ots` OpenTimestamps priority proofs
