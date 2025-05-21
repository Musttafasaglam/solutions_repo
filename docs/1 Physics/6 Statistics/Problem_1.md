#  Advanced Statistical Simulations

---

##  Problem 1: Exploring the Central Limit Theorem (CLT) Through Simulations

###  Overview and Historical Context

The **Central Limit Theorem** (CLT) is a fundamental result in probability theory that emerged in the 18th century with early insights from Abraham de Moivre, and was formalized by Pierre-Simon Laplace and later by Lyapunov. It underpins the reliability of the **normal distribution** in inferential statistics.

The theorem states:

> Given a population with finite mean $\mu$ and finite standard deviation $\sigma$, the sampling distribution of the sample mean $\bar{X}$ of size $n$ tends toward a normal distribution as $n$ becomes large, regardless of the population’s original distribution.


$$
\bar{X} \sim \mathcal{N}\left(\mu, \frac{\sigma^2}{n}\right)
$$

---

###  Experimental Setup

We simulate three population types:

- Uniform distribution $\mathcal{U}(0,1)$
- Exponential distribution $\text{Exp}(\lambda = 1)$
- Binomial distribution $\text{Bin}(n=10, p=0.5)$

We generate:
- A large population ($N = 100,000$ values)
- Sampling distributions for sample sizes $n = \{5, 10, 30, 50\}$

![alt text](image-4.png)
![alt text](image-8.png)
![alt text](image-6.png)
---



---

###  Real-World Implications

- **Survey analysis**: Estimating population opinions with confidence intervals.
- **Industrial quality control**: Using sample means to monitor process stability.
- **Machine Learning**: Underpins assumptions in regression and hypothesis testing.

---



---




