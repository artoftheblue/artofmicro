# Lecture 6, 08.10.2024

## Risk-averse people

Risk-averse people at initial $w=w^*$

$$u(w)=\ln w,\quad w>0$$

$$g=\left(\frac{1}{2}\circ(h),\frac{1}{2}\circ(-h)\right)$$

$$I_U=u(g)=\ln\sqrt{(w^*)^2-h^2}=\ln(CE)$$

$$\implies CE=\sqrt{(w^*)^2-h^2}<w^*$$

However if 

$$g_2=\left(\frac{1}{2}\circ(2n),\frac{1}{2}\circ(-2n)\right),\quad CE=\sqrt{(w^*)^2-4h^2}<CE$$

## Measure of risk aversion (Arrow-Pratt)

Measure of absolute risk aversion

$$R_a(w)=-\frac{-u(w)}{u(w)}$$

$$g=(p\circ x_1,(1-p)\circ x_2)$$

---

$$\boxed{u(w)=pu(x_1)+(1-p)u(x_2(x_1))}$$

At $(x_1, x_2)=(0, 0)$ I need to find $\frac{\partial x_2}{\partial x_1}$

$$0=pu'(x_1)+(1-p)u'(x_2)x_2'$$

$$x_2'=-\frac{p}{1-p}$$

$$px_1+(1-p)x_2=0$$

$$px_1+(1-p)x_2>0$$

$$\frac{\partial^2 x_2}{\partial x_1^2}\biggm|_{(0,0)}=?$$

$$0=pu''(x_1)+(1-p)u''(x_2)(x_2')^2+(1-p)\underbrace{u'(x_2)}_wx_2''$$

$$R_a(w)=\frac{u''(w)}{u'(w)}$$

$$0=pu''(w)+(1-p)u''(w)\frac{p^2}{(1-p)^2}+(1-p)u'(w)x_2''(0)$$

$$\boxed{-\frac{p}{(1-p)^2}\frac{u''(w)}{u'(w)}=x_2''(0)}$$

$$x_2''(0)=-\frac{p}{(1-p)^2}\cdot\frac{u''(w)}{u'(w)}$$

---

$$0<\alpha<1$$

$$u(w)=w^\alpha$$

$$R_a(w)=-\frac{\alpha(\alpha - 1)w^{\alpha-2}}{\alpha w^{\alpha-1}}=(1-\alpha)\frac{1}{w}$$

The following person's risk-aversion doesn't depend on wealth:

$$u(w)=-e^{-w\alpha}$$

$$u'=\alpha e^{-\alpha w},\quad u''=-\alpha^2e^{-\alpha w}$$

$$R_a(w)=\alpha$$

Very often risk-averse people are constructed as 

$$u(w)=\alpha w-\beta w^2,\quad\alpha,\beta>0$$

$$u'=a-2\beta w\quad u''=-2\beta$$

$$R_a(w)=\frac{2\beta}{\alpha-2\beta w}$$

Now let's prove the following theorem from the previous lecture

```{prf:theorem}
Two risk-averse individuals have $U(g)$ and $\nu(g)$ VNM functions, respectively.

Let their Arrow-Pratt measures $R_a^1(w)>R^2_a(w),\forall w\geq0$, where

$$R^1_a(w)=-\frac{U''(w)}{U'(w)}$$

and

$$R^2_a(w)=-\frac{\nu''(w)}{\nu'(w)}$$

Then there exists $C^2$ function $h(x)$ with $h''(x)<0$ for $x>0$ such that $U(w)=h(\nu(w))$.

Furthermore,

$CE_1<CE_2$ where $CE_1$ and $CE_2$ are their respective certainty equivalents.
```

```{prf:proof}

$$R^1_a(w)=-\frac{u''(w)}{u'(w)}>R^2_a(w)=-\frac{v''(w)}{v'(w)}$$

Let $h(x)=u(v^{-1}(x)),\quad x>0$

$$h'(x)=\frac{u'(v^{-1}(x))}{v'(x)}>0$$

$$\begin{align*}h''(x)&=\frac{v'(v^{-1}(x))\frac{u''(v^{-1}(x))}{v'(v^{-1}(x))}-u''(v^{-1}(x))\frac{v''(v^{-1}(x))}{v'(v^{-1}(x))}}{[v'(v^{-1}(x))]^2}
\\&=u'(v^{-1}(x))\frac{\left[\frac{u''}{u'}-\frac{v''}{v'}\right]}{(v'(v^{-1}(x)))^2}
\end{align*}$$

---

Using Jensen's inequality, we get

$$u(CE_1)=\sum^n_{i=1}p_ih(v(w_i))<h\left(\sum^k_1 p_1v(w_i)\right)=h(v(CE_2))=u(CE_2)$$

$$g=(p_1\circ w_1,\ldots,p_n\circ w_n)$$

$$h(tx_1+(1-t)x_2)>th(x_1)+(1-t)h(x_2)$$

Thus $CE_1<CE_2$ somehow...

```

## Applications of choice under uncertainty

### Problem of an investor

Let's sauppose that investor is risk-averse and his Arrow-Pratt measure $R_a(w)$ goes down with the rise in wealth. We'll call such individual as having the property of Decreasing Absolute Risk Aversion.

We consider such investor who solves the problem of the optimal investment to a risky asset. The neta rate of return is a random variable taking $n$ values both negative and positive with the probabilities $p_i$.

If $\beta$ wealth $(\beta < w)$ is chosen to invest into risky assets, then the expected utility maximization problem looks like 

$$\max_{0\leq\beta<w}\sum^n_{i=1}p_iU(w+\beta r_i)$$

Here $U(w)$ is an elementary utility function.

---

Initial wealth $w$ 

$0\leq\beta<w$ where $\beta$ is the part of wealth to be invested into a risky asset.

Let $r$ be the net rate of return.

$w-\beta+(1+r)\beta=w+\beta r$

Given DARA let $\beta^*$ be an optimal investment

$$\tilde r=\{r_i\}^n_{i=1}$$

then $\frac{\partial \beta^*}{\partial w}>0$.

$$Eu=\sum^n_{i=1}p_iu(w+\beta r_i)\to\max_{0\leq\beta<n}$$

$$\frac{\partial(Eu)}{\partial\beta}=\sum^n_{i=1}p_iu'(w+\beta r_i)r_i=0$$

$$\sum^n_{i=1}p_iu''(w+\beta r_i)r_i\left(1+\frac{\partial\beta^*}{\partial w}r_i\right)=0$$

$$\frac{\partial\beta^*}{\partial w}=-\frac{\displaystyle\sum^n_{i=1}p_iu''(w+\beta r_i)r_i}{\displaystyle\sum^n_{i=1}p_i u''(w+\beta r_i)r_i^2}$$

$$R_a(w+\beta r_i)=-\frac{u''(w+\beta r_i)}{u'(w+\beta r_i)}<-\frac{u''(w)}{u'(w)}r_i$$

$$u''(w+\beta r_i)r_i<-\frac{u''(w)}{u'(w)}r_i\cdot u'(w+\beta r_i)$$

Thus

$$\frac{\partial\beta^*}{\partial w}=-\frac{\displaystyle\sum^n_{i=1}p_iu''(w+\beta r_i)r_i}{\displaystyle\sum^n_{i=1}p_i u''(w+\beta r_i)r_i^2}<-\frac{\partial''(u)}{u'(u)}\frac{\displaystyle\sum^n_{i=1}r_iu'(w+\beta r_i)}{\displaystyle\sum^n_{i=1}p_iu''(w+\beta r_i)r_i^2}=0$$

However

$$\frac{\displaystyle\sum^n_{i=1}p_iu''(w+\beta r_i)r_i}{\displaystyle\sum^n_{i=1}p_i u''(w+\beta r_i)r_i^2}>0$$

Thus we're done.

---

```{prf:proposition}
Let $U'>0,U''<0$ and an agent satisfies the property of DARA. Then, $\frac{\partial\beta}{\partial w}>0,\beta$ is the risky investment.
```

### Application 2

Suppose that the probability of an accident that implies a loss of a property or a car is $p$.

If the cost of unit of the insurance coverage $\alpha$ equals $p$, we say that the insurance is actuarially fair.

Let $p=\alpha$ and a risk-averse individual with the elementary utility function $U(w)$ must decide for how much to insure his car.

We assume that his wealth is $w$ and the cost of the car $L<w$. How much insurance $x$ will he buy?

$$E\pi=(1-p)\alpha+p(\alpha-1)=0$$

```{prf:proposition}
Let $U(w)$ be an elementary utility function with $U'>0, U''<0$, and the insurance is actuarially fair, then he buys insurance $x=L$, i. e. the coverage is full.
```

```{prf:proof}

$$Eu=pu(w-\alpha x-L+x)+(1-p)u(w-\alpha x)\to\max_{0<x\leq L}$$

$$(E_u)'_x=pu'(w-\alpha x-L+x)(1-\alpha)-(1-p)u'(w-\alpha x)\alpha=0$$

$$\alpha=p$$

$$u'(w-\alpha x-L+x)=u'(w-\alpha x)$$

$$w-\alpha x-L+x=w-\alpha x$$

$$x=L$$

```

## Contingent goods

Contingent goods help to account for the random events, such as a university entry with a full tuition waiver, and for our exposition, we'll talk about insurance and risk investments.

So, we look at a 2-stage game and the nature plays with us. For example, when I insure my car, I cover insurance with the payment, hoping that an accident will not occur. But with the (objective) probability it occurs.

So, state of nature (or world) is the set $S=\{1,2,\dots,\hat s\}$ in the second stage with the probability of $\mu_s\geq 0$ state $x_s$ occurs.

Then, if the elementary utility is $U(w)$, we define the VNM function as 

$$\mathbb{E} U=\sum_{s\in S}\mu_s U(w_s)$$

The same definition as in the axiomatic approach.

```{prf:example}
Let $y$ denote the converage of a loss in the amount of $L$. The insurance premium per 1 dollar is $0<\gamma<1$, and the probability of a loss is $p$. Clearly, $\gamma\geq p$ (if $\gamma=p$, we are in an actuarially fair case).

If we have two states of nature, ($L$ — loss, $NL$ — no loss), then denoting the wealth as $x_L$ and $x_{NL}$, we get VNM function as $pU(x_L)+(1-p)U(x_{NL})$

Here $x_L=w-\gamma y-L+y$ and $x_{NL}=w-\gamma y$.

Then, we have the following problem

$$\begin{cases}
    pU(x_L) + (1- p)U(x_{NL})\to\max\\
    \text{given that } (1-\gamma)x_{NL}+\gamma x_L=w-\gamma L
\end{cases}$$
```

$$(1-\gamma)x_{NL}+\gamma x_L=w-\gamma L$$

$$-\frac{\gamma}{1-\gamma}$$

$$x_{NL}=x_L=w-\gamma L$$

$$pu(x_2)+(1-p)u(x_{NL})\to\max_{x_L, x_{NL}\geq 0}$$

$$MRS_{x_L, x_{NL}}=\frac{pu'(x_L)}{(1-p)u'(x_{NL})}=\frac{\gamma}{1-\gamma}$$

$$x_L=x_{NL}$$

$$\gamma>p\implies MRS<\frac{p}{1-p}<\frac{\gamma}{1-\gamma}$$

```{figure} ./image-27.png
:height: 300
:label: figure-img-27
Something that was on the board
```

$x \cdot r$, $r_g$ — gross, $x(1+r_n)=x+xr_n$.

```{prf:proposition}
If the insurance of a risk-averse individual is actuarially unfair $(\gamma > p)$, then $0\leq y<L$, where $y$ is the insurance coverage.
```

## Handling risky investments

Let a risk-averse investor have $w$ wealth, which can be distibuted between $l$ risky assets whose rates of return are random and one non-risky asset (e. g. deposit in a bank).

So, if $k\geq 1, r_k$ is random. Here $k\in K=\{1,\ldots,l\}$.

The states of nature are from $S=\{1,\ldots,\hat s\}$, and their probabilities are $\mu_s\geq 0,\quad \sum_{s\in S}\mu_s=1$.

Given the gross rate of return $\tilde r_k$, it takes the values $\{r_{k_s}\}^{\hat s}_{s=1}$.

If the random wealth is $\tilde x$, then $\displaystyle\tilde x =r_0z_0+\sum^l_{k=1}z_k\tilde r_k$, where $r_0$ is a non-risky return.

$$\alpha_0=1-\sum^l_{i=1}\alpha_i$$

$$\alpha_i=\frac{z_i}{w}$$

Let $\alpha_0=\frac{z_0}{w}$ and $\alpha_k=\frac{z_k}{w}$

Expected utility 

$$\mathbb{E}U\left(w\left(r_0+\sum_{k\geq 1}\alpha_k(\tilde r_k-r_0)\right)\right)$$

will be maximized with respect to $\alpha_k$. 

For simplicity, we may consider just one risky asset with $\tilde r_1$ return.

---

$$\mathbb{E}u(\underbrace{w(r_0+\alpha_1(r_1-r_0))}_{\tilde x})\to\max_{\alpha_1\geq 0}$$

$$\frac{\partial(\mathbb{E}u)}{\partial\alpha_1}=[\mathbb{E}u'(\tilde x)w(r_1-r_0)]\biggm|_{\alpha_1=0}\leq 0$$

$$\mathbb{E}\tilde r_1\leq r_0$$

no investment

Let $\alpha_1>0$, then

$$E(u'(\tilde x)(\tilde r_1-r_0))=0$$

$$E(u'(\tilde x)\tilde r_1)-(Eu'(\tilde x))r_0=0$$

$$cov(\xi,\eta)=\mathbb{E}[(\xi-\mathbb{E}\xi)(\eta-\mathbb{E})]=\mathbb{E}(\xi\eta)-\mathbb{E}\xi\cdot\mathbb{E}\eta<0$$

$$\mathbb{E}u'(\tilde x)\mathbb{E}\tilde r_1>\mathbb{E}(u'(\tilde x)\tilde r_1)=r_0\mathbb{E}u'(\tilde x)$$

$$\mathbb{E}\tilde r_1>r_0$$

---

```{prf:proposition}
In the investor's problem described above, the $\alpha_1>0\iff\mathbb{E}\tilde r_1>r_0$.  

More general result was proven by Samuelson.
```

```{prf:theorem}
Let investor characterized by the elementary utility function $U(w)$, with $U'>0,U''<0$, the assets are statistically independent, $\alpha_0$ can have any sign, and each return $\tilde r_k$ is a discrete random variable.

Then, any risky asset $k\in K$, whose expected return $\mathbb{R}\tilde r_k$ is greater than $r_0$, will be bought. 
```

## Moral hazard in insurance

Incentive to drive carefully diminishes with the amount of coverage. Let an insurance company be a monopolist in the market. A car accident may result in varying amounts of loss.

$0\leq l\leq L$ — maximum loss (still less than $W$). Effort of a driver to drive carefully takes 2 values, 0 and 1.

The probability of an accident $\pi_l(e)$, $l$ — damage, $e$ — effort.

$$\sum_{l=0}^L\pi_l(1)=1,\quad\sum^L_{l=0}\pi_l(0)=1$$

Assumption on probabilities property $\frac{\pi_l(0)}{\pi_l(1)}$ is strictly increasing in $l$ from $0$ to $l$. It's called the monotone likelihood. More on this!

Let the reservation utility be $\bar u$ (what if an agent refuses to insure?)

$$p-\sum^L_{l=0}\pi_l(e)B_e\to\max_{p,l,B_l}$$

$e$ is chosen by the company such that 

$$\sum^L_{l=0}\pi_l(e)u(w-p-l+B_l)-d(e)\geq \bar u$$

than reckless driving $\implies$ disutility $d(e)$, $d(1)>d(0)$.

Effort not seen by the company. Damage is seen. Let $B_l\geq 0$ be the coverage in case of the $l$ damage. Clearly, $B_l\leq l$.
