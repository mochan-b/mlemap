---
---

# Introduction to MLE and MAP

---

# Bayes Rule for random variables

- Given that $X$ and $\Theta$ are random variables,

$$
f_{\Theta|X}(\theta|x) = \frac{f_{X|\Theta}(x|\theta) f_\Theta(\theta)}{f_X(x)}
$$

- Based directly off from the Bayes theorem for sets and probability.

---

# Basic Probability

- Probability triplet: $(\Omega, \mathcal{F}, P)$
   - $\Omega$ is a set
   - $\mathcal{F}$ is a set of some subsets of $\Omega$
   - $P$ is a function such that for $A \in \mathcal{F}$, $P(A) \in [0,1]$
- Random Variable $X$ is a function
$$
X : \Omega \rightarrow \mathbb{R} \; (\text{or something similar})
$$
and we denote $P(X=x)$ or $P_X(x)$ as 
$$
P_X(x) = \{ \omega \in \Omega, X(\omega) = x \}
$$

---

# Conditional Probability

- Given $A, B \in \mathcal{F}$, 
$$
P(A|B) = \frac{P(A \cap B)}{P(B)}
$$
- For random variables $X$ and $Y$, 
$$
f_{Y|X}(y|x) = \frac{f_{X,Y}(x,y)}{f_X(x)}
$$

---

# Likelihood

- Let $\mathbf{x} = x_1, \ldots, x_n$ be our data set. We have a family of distribution that we guess our data comes from. Let $\theta$ be our estimate of the best fit parameter of our distribution.
- Likelihood gives the probability of $\theta$ matching the data $\mathbf{x}$
$$
\mathcal{L}(\theta | \mathbf{x})
$$
- Using Bayes theorem, we have
$$
\mathcal{L}_{\Theta|X} (\theta | x) = f_{X|\Theta}(\mathbf{x} | \theta) \frac{f_\Theta(\theta)}{f_X(\mathbf{x})}
$$

---

