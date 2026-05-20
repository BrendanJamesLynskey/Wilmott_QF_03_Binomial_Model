# The Binomial Model

Deck 03 of the [Paul Wilmott Introduces Quantitative Finance &mdash; Companion Series](https://github.com/BrendanJamesLynskey/Wilmott_QF_Hub).

**Live presentation:** https://brendanjameslynskey.github.io/Wilmott_QF_03_Binomial_Model/

A guided tour of chapter 3 of *Paul Wilmott Introduces Quantitative Finance*
(2nd edition, Wiley, 2007) &mdash; the first proper *model* in the book: a
two-state random walk for the share price, no-arbitrage hedging at every node,
and the risk-neutral pricing recipe that converges to Black&ndash;Scholes.

## What's inside

- The one-step setup: $S \to uS$ or $S \to dS$, the no-arbitrage condition $d < 1 + r\delta t < u$
- Delta hedging in the tree: $\Delta = (V^+ - V^-)/(uS - dS)$
- The backward equation $V = (p' V^+ + (1-p') V^-)/(1+r\delta t)$ and the risk-neutral probability $p'$
- Why the real-world probability $p$ never appears
- Multi-step recombining lattice and the $S_n^{(j)} = S_0 u^j d^{n-j}$ node formula
- Backward induction with a worked 3-step European call
- Greeks (delta, gamma, theta) read off the tree as finite differences
- American options as a Bellman recursion: $V = \max(\text{intrinsic}, \text{continuation})$ and the early-exercise boundary
- CRR convergence to geometric Brownian motion and the Black&ndash;Scholes price
- **Interactive binomial tree pricer** &mdash; sliders for $S_0$, $K$, $r$, $\sigma$, $T$, $N$; toggles for European/American and call/put; tree drawn live with node radius scaled by stock price and colour heatmapped by option value; metrics show $u$, $d$, $p'$, the option price, initial delta and a Black&ndash;Scholes reference

Companion to chapter 3 of:

> Wilmott, P. (2007). *Paul Wilmott Introduces Quantitative Finance,
> Second Edition.* John Wiley &amp; Sons. ISBN 978-0-470-31958-1.

Single-page HTML, KaTeX-rendered maths, no build step. Open `index.html` directly.
