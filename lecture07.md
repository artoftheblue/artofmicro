# Lecture 7, 15.10.2024

> Start of this lecture duplicates starting from [this example](#ref6) and further.

## Moral hazard in insurance

Incentive to drive carefully diminishes with the amount of coverage. Let an insurance company be a monopolist in the market. A car accident may result in varying amounts of loss.

$0\leq l\leq L$ — maximum loss (still less than $W$). Effort of a driver to drive carefully takes 2 values, 0 and 1.

The probability of an accident $\pi_l(e)$, $l$ — damage, $e$ — effort.

$$\sum_{l=0}^L\pi_l(1)=1,\quad\sum^L_{l=0}\pi_l(0)=1$$

Assumption on probabilities property $\frac{\pi_l(0)}{\pi_l(1)}$ is strictly increasing in $l$ from $0$ to $l$. It's called the monotone likelihood. More on this!

---

Profit maximization

$p$ — price of the contract

$$p-\sum_{l=0}^L\pi_l(e)B_l\to\max_{p, B_l}$$

such that 

$$\sum^L_{l=0}\pi_l(e)u(w-p-l+b_l)-d(e)\geq \bar u$$

$$\mathcal{L}=p-\sum_{l=0}^L\pi_l(e)B_k-\lambda\left[\sum_{l=0}^L\pi_l(e)U(w-p-l-B_l)\right]$$

$$\frac{\partial\mathcal{L}}{\partial p}=1-\lambda\sum^L_{l=0}\pi_l(e)u'(w-p-l+B_l)=0$$

$$\frac{\partial\mathcal{L}}{\partial B_l}=\cancel{-\pi_l(e)}+\lambda\cancel{\pi_l(e)}u'(w-p-l+B_l)=0$$

$$0\leq l\leq L$$

$$u'(w-p-l+B_l)=\frac{1}{\lambda}=\text{const}$$

$$l=0,\quad B_0=0,\quad \boxed{B_l=l}$$

We say that this is full coverage.

$$u(w-p)=d(e)+\bar u,\quad d(1)>d(0)$$

$p$ for $l=0$ is bigger than for $e=1$.

$$\text{Profit}=p-\sum^L_{l=0}\pi_l(e)l$$

```{seealso} Exercise
$$\sum^L_{l=0}\pi_l(0)l>\sum^L_{l=0}\pi_l(1)l$$
```
---

Now we are in the situation of assymetric information.

$$\begin{align*}&\sum_{l=0}^L\pi_l(e)u(w-p-l+B_l)-d(e)\\\geq&\sum^L_{l=0}\pi_l(e')u(w-p-l+B_l)-d(e')\end{align*}$$

$$e=0, \quad e'=1,\quad u(w-p)-d(0)\geq u(w-p)-d(1)\implies d(0)>d(1)$$

Now check when there is interest in hazardous driving:

$$e=1, \quad e'=0$$

$$\mathcal{L}=p-\sum^L_{l=0}\pi_l(1)B_l+\lambda\left[\sum^L_{l=0}\pi_l(1)u(w-p-l+b_l)-d(1)-\bar u\right]\\+\,\mu\left[\sum^L_{l=0}(\pi_l(1)-\pi_l(0))u(w-p-l+B_l)+d(0)-d(1)\right]$$

$$-\mu\left[\sum^L_{l=0}(\pi_l(1)-\pi_l(0))u'(w-p-l+B_l)\right]=0$$

$$\frac{\partial\mathcal{L}}{\partial B_l}=-\pi_l(1)+\lambda\pi_l(1)u'(w-p-l+B_l)+\\\mu(\pi_l(1)-\pi_l(0))u'(w-p-l+B_l)=0$$

We know that $\lambda\geq 0,\mu\geq 0$

$\frac{\pi_l(0)}{\pi_l(1)}$ with rise in l, monotony likelihood function.

$$\lambda u'(w-p-l+B_l)+\mu\left(1-\frac{\pi_l(0)}{\pi_l(1)}\right)u'(w-p-l+B_l)$$

$$\boxed{\lambda+\mu\left(1-\frac{\pi_l(0)}{\pi_l(1)}=\frac{1}{u'(w-p-l+B_l)}\right)}$$

If $\lambda\geq0,\mu\geq0\implies l=B_l\implies\lambda,\mu>0$

---


```{seealso} I managed to copy this from the paper but idk what it refers to
Let the reservation utility be $\bar u$ (what if an agent refuses to insure?)

$$p-\sum^L_{l=0}\pi_l(e)B_e\to\max_{p,l,B_l}$$

$e$ is chosen by the company such that 

$$\sum^L_{l=0}\pi_l(e)u(w-p-l+B_l)-d(e)\geq \bar u$$

than reckless driving $\implies$ disutility $d(e)$, $d(1)>d(0)$.

Effort not seen by the company. Damage is seen. Let $B_l\geq 0$ be the coverage in case of the $l$ damage. Clearly, $B_l\leq l$.
```

## Problem 4

Innovative firm seels the patent to the two simulatenously competing firms whose costs are $TC_i=cq_i^2+FC_i, i=\overline{1,2}$. These firms pay royalty $\rho$ per unit sold and no lump sum rotalty is charged.

### Subproblem A

Let these firms face $p(Q)=1-Q$ demand, find the $\rho$ value that enables the firms to sustain monopoly price.

---

$$\pi_1+\pi_2=(1-Q)Q-2c\left(\frac{Q}{2}\right)^2\to\max_{Q>0}$$

$$FOC: 1-2Q-cQ=0$$

$$Q^m=\frac{1}{c+2},\quad p^m=1-\frac{1}{c+2}=\frac{c+1}{c+2}$$

$$\pi_1=(1-q_1-q_2)q_1-\rho q_1-cq_1^2\to\max_{q_1\geq0}$$

$$1-2q_1-q_2-\rho-2cq_1=0$$

Symmetrical equilibrium $\implies$

$$q_1^*=q_2^*=q^*=\frac{1-\rho}{3+2c}$$

$$1-\rho=(3+2c)q^*,\quad 2q^*=\boxed{\frac{2-2\rho}{3+2c}=\frac{1}{c+2}}$$

$$(2-2\rho)(c+2)=3+2c$$

$$2c+4-2\rho(c+2)=3+2c$$

$$1=2\rho(c+2)$$

$$\boxed{\rho^*=\frac{1}{2(c+2)}}$$

### Subproblem B

Let's suppose that agreement was signed only by the second firm, and the patent holder has to produce itself. Given $TC(q)=cq^2$, find under what royalty value the firms will charge the price as in Subproblem A.

---

$$\tilde\pi=(1-\tilde q-q)\tilde q+\rho q-c\tilde q^2\to\max_{\tilde q\geq0}$$

1. $$\frac{\partial\tilde \pi}{\partial\tilde q}=1-2\tilde q-q-2c\tilde q=0$$

    $$\pi=(1-\tilde q-q) q-\rho q-cq^2\to\max_{q\geq 0}$$

2. $$\frac{\partial \pi}{\partial q}=1-\tilde q-2q-\rho-2cq=0$$

$$\begin{cases}
    (2c+2)\tilde q+q=1\\
    \tilde q+(2c+2)q=1-\rho
\end{cases}$$

$$\begin{cases}
    \tilde q +(2c+2)q=1-\rho\\
    \tilde q+\frac{q}{2c+2}=\frac{1}{2c+2}
\end{cases}$$

$$\left[(2c+2)-\frac{1}{2c+2}\right]q=1-\rho-\frac{1}{2c+2}$$

$$(2c+3)(2c+1)q=(2c+2)(1-\rho)-1=2c+2-\rho(2c+2)-1$$

$$q=\frac{(1-\rho)(2c+2)-1}{(2c+3)(2c+1)}$$

$$\begin{align*}\tilde q&=1-\rho-\left[\frac{(1-\rho)(2c+2)-1}{(2c+1)(2c+3)}\right](2c+2)+\frac{(1-\rho)(2c+2)-1}{(2c+3)(2c+1)}
\\&=1-\rho-\frac{[(1-\rho)(2c+2)-1]}{2c+1}=\frac{1}{c+2}
\end{align*}$$

$$(1-\rho)\left[1-\frac{2c+2}{2c+3}\right]=\frac{1}{c+1}-\frac{1}{2c+3}$$

$$(1-\rho)\frac{1}{2c+3}=\frac{c+1}{(c+2)(2c+3)}$$

$$2c^2+5c+2-2c-2$$

$$2c^2+3c$$

## Problem 5

Two producers of the dental cream compete a la Bertrand. Demand is given by $q_i=1-p_i+\tfrac{1}{2}p_{-i}$, where $i=1,2$.

Let $MC_i=0$ and there are no fixed costs.

### Subproblem A

Find the Bertrand equilibrium in this game.

---

Firm 1: $q_1=1-p_1+\frac{1}{2}p_2$

$$p_1q_1\to\max_{p_1>0},\quad p_1q_1=p_1-p_1^2+\frac{1}{2}p_2p_1\to\max$$

$$0=1-2p_1+\frac{1}{2}p_2=0$$

Best response is 

$$1+\frac{1}{2}p_2=2p_1$$

$$p_1=BR_1(p_2)\frac{1}{2}+\frac{1}{4}p_2$$

Firm 2: $q_2=1-p_2+\frac{1}{2}p_1$

$$p_2q_2=p_2-p_2^2+\frac{1}{2}p_1p_2$$

$$\frac{\partial(p_2q_2)}{\partial p_2}=1-2p_2+\frac{1}{2}p_1=0$$

$$p_2=BR_2(p_1)=\frac{1}{2}+\frac{1}{4}p_1$$

$$p_1^*=p_2^*=\frac{2}{3}$$

```{figure} ./image-28.png
:label: something
Nash equilibirium
```

$$p_1q_1=p_1\left(1-p_1+\frac{1}{4}+\frac{1}{8}p_1\right)\to\max_{p_1>0}$$

$$p_1\left(\frac{5}{4}-\frac{7}{8}p_1\right)\to\max$$

$$\frac{5}{4}-\frac{7}{4}p_1^*=0\implies p_1^*=\frac{5}{7}$$

$$p_2^*=\frac{1}{2}+\frac{5}{28}=\frac{19}{28}>\frac{2}{3}$$

$$q_1=q_2=1-\frac{2}{3}+\frac{1}{3}=\frac{2}{3}$$

$$\pi_1=\pi_2=\frac{4}{9}$$

$$\tilde q_1=1-\frac{5}{7}+\frac{19}{56}=\frac{2}{7}+\frac{19}{56}=\frac{16+19}{56}=\frac{35}{56}<\frac{4}{9}$$

$$\tilde q_2=1-\frac{19}{28}+\frac{5}{14}=\frac{28-19+10}{28}=\frac{19}{28}$$

$$$$

### Subproblem B

Consider a two-stage game, when firm 1 is the leader that knows the best response of the follower. Solve this game and compare profits obtained in these games.

## Problem 9

Risk averse individuals are of the two types. Agents of the first type have utility function $U^1(w)=-w^{-\frac{1}{2}}$, and the rest have $U^2(w)=-w^{-1}$. These two types differ in their attitude toward parking payment. Parking by the mall costs $p$ euros. All these individuals have $w$, money wealth that $w>2p$. According to their type, some of the drivers do not pay at and they do not mind to pay fine, the other drivers are indffferent between paying or not paying the fee. The probability to be caught with no ticket is $\frac{2}{5}$. If such person is caught, they should pay the fee plus the fine which is also $p$ euros.

Calculate the minimal probability of capture such that if the true probability exceed this threshold value, the behaviour of the agents will change and those who declined to pay will become indifferent towards payment or no payment.

---

$$R^1_a=-\frac{(-\frac{1}{2})(-\frac{3}{2})}{-\frac{1}{2}}\frac{1}{w}=\frac{3}{2w}$$

$$R^2_a=-\frac{(-1)(-2)}{(-1)}\frac{1}{w}=\frac{2}{w}>\frac{3}{2w}$$

$$U_2(w)=-\frac{1}{w}$$

$$-\frac{1}{w-p}=-\frac{\frac{3}{5}}{w}-\frac{\frac{2}{5}}{w-2p}$$

$$\frac{1}{w-p}=\frac{\frac{3}{5}}{w}+\frac{\frac{2}{5}}{w-2p}$$

$$\frac{w}{w-p}-\frac{\frac{2}{5}w}{w-2p}=\frac{3}{5}$$

$$w(w-2p)-\frac{2}{5}w(w-p)=\frac{3}{5}(w-p)(w-2p)$$

$$w^2-2pw-\frac{2}{5}w^2+\frac{2}{5}wp=\frac{3}{5}(w^2+2p^2-3pw)$$

$$-\frac{8}{5}pw=\frac{3}{5}(2p^2-3pw)$$

$$6p^2-$$

---

$$U_1=-\frac{1}{\sqrt{w}}$$

$$-\frac{1}{\sqrt{w-p}}=-\frac{\gamma}{\sqrt{w}}-\frac{(1-\gamma)}{\sqrt{w-2p}}$$

$$\frac{1}{\sqrt{\frac{5}{6}}}=\gamma+\frac{1-\gamma}{\sqrt{\frac{2}{3}}}$$

$$\sqrt{\frac{6}{5}}=\gamma+(1-\gamma)\sqrt{\frac{3}{2}}$$

$$\sqrt{\frac{6}{5}}=\gamma +\sqrt{\frac{3}{2}}-\gamma\sqrt{\frac{3}{2}}$$

$$\gamma\left(\sqrt{\frac{3}{2}}-1\right)=\sqrt{\frac{3}{2}}-\sqrt{\frac{6}{5}}$$

$$\gamma^*=\frac{\sqrt{\frac{3}{2}}-\sqrt{\frac{6}{5}}}{\sqrt{\frac{3}{2}-1}}$$

## Problem 7

> Sorry no extensive solutions because I'm too tired to filter information and we solved these tasks mostly orally.

Maria's income is $100$ dollars. If she gets sick, then her income becomes $49$ dollars. The probability of sickness is $\frac{1}{3}$. Her elementary utility function is $U=\sqrt{w}$, where $w$ is her wealth. The insurance company is neutral to risks and it proposes Maria to insure her against the illness.

### Subproblem A

What is the maximum insurance premium Maria is willing to pay?

---

```{figure} ./image-30.png
:name: something
Graph for the solution.
```

$$EU=\frac{1}{3}\cdot7+\frac{2}{3}\cdot10=9=\sqrt{81}$$

$$100-81=19$$

### Subproblem B

Maria thinks about her insurance proposal. What would be the minimal premium this company agrees to offer?

---

$$(100-49)\frac{1}{3}=\frac{51}{3}=17$$

### Subproblem C

Michael is identical to Maria in terms of wealth, utility and health. If they agree to split equally the income when only one of them falls sick would this risk sharing be beneficial for them both? Explain.

---


