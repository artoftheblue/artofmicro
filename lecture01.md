# Classic monopoly

## Definition

```{prf:definition}
A firm is **a monopoly** if no other firms produces the same good or a close substitute.
```

```{note} 
We differentiate among the products referring to the cross-price elasticity: if its value is small, then the potential substitutes are not close enough to be a substitute.
```

A monopolist has market power in the sense that the amount of output that it is able to sell responds continuously to the price it charges.

Obviously, the monopolist offers consumers some good at price $p$. 

## Monopoly Examples

```{prf:example}
The main reason why a monopoly exists is the fact that other firms find it impossible or unprofitable to enter the market (or to continue competing with larger firms).

The most striking examples of monopolies are:

1. **Natural monopolies** — a single company can produce and offer to sell a product or service at a lower cost than its competitors can.
2. **Legal protection of a patent holder** — the government prohibits some technologies, ideas and production methods to be used by anyone except for their creators.
```

## Monopoly Model

Let's suppose there are many consumers of a good, and they are price-takers. We'll assume that a good which we're considering is normal, which means that the function of demand $D(p)$ is decreasing.

The market demand is given by $y=D(p)$ — the output of the monopoly, $c(y)$ — costs function of the firm-monopolist.

So, the monopolist chooses the price $p^m$, which is the solution of the maximization problem:

(eq1.3.1)=
$$
\Pi(p)=pD(p)-c(D(p))\longrightarrow\max_{p\geqslant0}
$$

Logically, $y^m=D(p^m)$ is the output of the monopolist.

Sometimes it's easier to use an inverse function $p=p(y)=D^{-1}(y)$.

Then, output $y^m$ is the solution of this problem:
\begin{equation}\label{eq:1.3.2}
\Pi(y)=p(y)y-c(y)\longrightarrow\max_{y\geqslant0}
\end{equation}

## First-order condition
\begin{equation}
\begin{cases}
\Pi'(y^m)\leqslant 0\\
y^m\cdot\Pi(y^m)=0
\end{cases}
\end{equation}
\indent Condition that $y^m>0$ is guaranteed by:
\begin{equation}
p(0)>c'(0)
\end{equation}

**Proof.** If $y^m=0$, next condition must be done:
\begin{equation*}
\Pi'(0)=p(0)-c'(0)\leqslant 0
\end{equation*}
which contradicts $p(0)>c'(0)$\qed

\begin{equation}
\begin{aligned}
\Pi(y)&=p(y)y-c(y)\\
\Pi'(y)&=\left(p(y)y-c(y)\right)^{\prime}=0\\
&=p(y)\cdot p'(y)y=c'(y),\quad \text{at }y=y^m>0
\end{aligned}
\end{equation}

Then, $p^m=p(y^m)$

Let's $TC=D(p)p$, $TC=c(D(p))$, then as we maximize $\Pi$
\begin{equation*}
\begin{aligned}
\Pi'&=0\\
TR'-TC'&=0\\
MR-MC&=0
\end{aligned}
\end{equation*}

```{figure} ./image-1.png
:label: image1
:height: 400
:align: center

Visualization of the case when $MC=MR$.
```

## Second-order condition
Let $TR(y)=p(y)y$ and $MR(y)=TR'(y)$, then
\begin{equation}
\left(MR(y^m)\right)'<\left(MC(y^m)\right)'
\end{equation}
## Illustration of the monopolist problem

```{figure} ./image-2.png
:label: image2
:height: 400
:align: center

Illustration of the monopolist problem
```

Here $p^m$ and $y^m$ are the price and output at which customers will buy the volume of good at which $MR=MC$.

## Inverse elasticity pricing rule
\definition 
\begin{equation}\label{eq:1.7.1}
\frac{p^m-MC(y^m)}{p^m}=\frac{1}{|\varepsilon_d|},\quad \text{for }|\varepsilon_d|>1
\end{equation}

The right part of the formula ([](#eq:1.7.1)) is called **Lerner's Index**. It shows the degree of the monopoly power. At the same time it shows how the mark-up price depends on the elasticity of demand. 

\comment If the elasticity of demand is infinite, then the firm is a price taker and has no market power.

\comment The greater the elasticity, the smaller the markup the manufacturer can make because in that case customers will refuse to consume.

Let's find the formula ([](#eq:1.7.1)) by mathematical transformation. We know that:

3. $p'(y^m)y^m+p(y^m)=c'(y^m)$
4. $p(y^m)=c'(y^m)$
5. $\varepsilon_d=\displaystyle\frac{\text{d}y}{\text{d} p}\cdot\frac{p}{y}<0$
\end{itemize}
So, transform by using that equations we get
$$\begin{aligned}
p(y^m)\left[1+\displaystyle\frac{p'(y^m)y^m}{p(y^m)}\right]&=c'(y^m)\\
p^m\left[1-\displaystyle\frac{1}{|\varepsilon_d|}\right]&=c'(y^m)\\
p^m-\displaystyle\frac{p^m}{|\varepsilon_d|}&=c'(y^m)\\
\displaystyle\frac{p^m-c'(y^m)}{p^m}&=\frac{1}{|\varepsilon_d|}\\
\frac{p^m-MC(y^m)}{p^m}&=\frac{1}{|\varepsilon_d|}
\end{aligned}$$

## Monopoly's output in comparison with the perfectly competitive industry
Consider a monopoly with the $c(y) \in C^1$ costs function and a perfectly competitive industry with the same costs $c(y)$.Let $p(y) \in C^1$ be an inverse demand function. Then given $p' > 0,\ c' > 0,\ c'' > 0$ and $p(0) > c'(0)$

\proposition The monopoly output $y^m$ will be less than the output $\overline{y}$ of the perfectly competitive industry
\begin{equation}\label{eq:1.8.1}
y^m<\overline{y}
\end{equation}

\proof It's simple. On the one hand, $y^m$ maximizes $\Pi$ of the monopoly, then
$$p(y^m)y^m-c(y^m)\geqslant p(\overline{y})\overline{y}-c(\overline{y})$$

On the other hand, $\overline{y}$ provides maximum profit to the price-taking firm at a constant price $p(\overline{y})$, then
$$p(\ov{y})\ov{y}-c(\ov{y})\geqslant p(\ov{y})y^m-c(y^m)$$

Adding these equations we get $p(y^m)y^m\geqslant p(\ov{y})y^m\Longrightarrow\boxed{y^m<\ov{y}}$\footnote{Remember, that $p(y)$ is an inverse function of demand and $y^m\ne \ov{y}$ because of $p(\ov{y})-c'(\ov{y})\leqslant0$}


```{figure} ./image-3.png
:label: image3
:height: 400
:align: center

Label
```

## Comparative Statics
Let $p(y)\in C^2,\ p' <0,\ MC =c,\ p(0)>c,\ (MR)' <0$. Then
\begin{equation*}
\frac{dy^m(c)}{dc}<0\quad \text{and}\quad\frac{dp^m(c)}{dc}>0
\end{equation*}

# Quasilinear Economy
Consider an economy where there are $m$ consumers and $n$ firms. All of consumers have quasilinear preferences, for $i$-th consumer his utility is $U_i(x_i,z_i)=v_i(x_i)+z_i$, where $x_i$ is the only good to be consumed and $z_i$ is the money owned by this consumer.

Properties of $v_i(x_i)$ functions:

6. $v_i'(x_i)>0$
7. $v_i''(x_i)<0$
8. $v_i(0)=0$
\end{itemize}

## Main theorem of the quasilinear economy
Let $\bar{x}=\left(x_1, x_2, \ldots, x_m\right), \bar{y}=\left(y_1, y_2, \ldots, y_n\right), \bar{r}=\left(r_1, r_2, \ldots, r_n\right)$ and $\bar{z}=\left(z_1, z_2, \ldots, z_m\right)$

Allocation $(\widehat{\bar{x}}, \widehat{\bar{y}}, \widehat{\hat{r}}, \widehat{\bar{z}})$ is Pareto-optimal if and only if it is a solution of the problem
\begin{equation}\label{eq:2.1.1}
\left\{\begin{array}{l}
\sum_i \nu_i\left(x_i\right)-\sum_j c_j\left(y_j\right) \longrightarrow \max \\
\sum_i\left(x_i\right) \leq \sum_i y_j \\
x_i \geq 0,\ y_j \geq 0 \\
\text {for all } i \in I \text { and } j \in J
\end{array}\right.
\end{equation}


Moreover $\widehat{r_j}=c_j\left(\widehat{y_j}\right)$ and $\sum_i \widehat{z_i}=\sum_i w_i-\sum_j \widehat{r_j}$.

## Welfare analysis under monopoly
The first line in ([](#eq:2.1.1)) is the main goal of consumers, i.e. to maximize the welfare. That function is called a **welfare indicator**. Then we have $2$ sets of indices, $I = \{1,2,\ldots,m\}$ and
$J = \{1,2,\ldots,n\}$.

At **Pareto-optimal allocation** it takes the maximum value $W_{max}$. If an allocation **is not** Pareto-optimal, then $W < W_{max}$ and this difference $W_{max} - W$ is called **deadweight loss** $(DWL)$.

We give the following definitions for Consumers’ ($CS$) and producers’ ($PS$) surplus:
\begin{equation}
\begin{aligned}
CS&=&\sum_{i\in I}\nu_i(x_i)-p\sum_{i\in I}x_i\\
PS&=&p\sum_{j\in J}y_j-\sum_{j\in J}c_j(y_j)
\end{aligned}
\end{equation}

Welfare indicator at $(x, y)$ allocation equals $W (x, y) = CS + PS$. Moreover, we can identify $$W=\sum_{i=1}^m v_i(x_i)-c(y)$$

Let $y=\sum_{i\in I}x_i=x$ — output of a monopoly


9. $W(y)=v(y)-c(y)\longrightarrow\max\limits_{y>0}\Longrightarrow v'(y)=c'(y)$
10. First-order condition:
\begin{equation*}
\begin{aligned}
\left(p(y)y\right)'-c'(y)&=0\\
p'(y)y+p(y)-c'(y)&=0
\end{aligned}
\end{equation*}
11. If we differentiate the formula $W(y)=v(y)-c(y)$:
\begin{equation*}
\begin{aligned}
W'(y^m)&=v'(y^m)-c'(y^m)>0\\
&=p(y^m)-c'(y^m)\\
&=-p'(y^m)y^m>0
\end{aligned}
\end{equation*}



```{figure} ./image-4.png
:label: image4
:height: 300
:align: center

Label
```

## DWL formula

```{figure} ./image-5.png
:label: image5
:height: 400
:align: center

Label
```

For instance, we have $p(y)=a-by$ and $c'(y)=c$ then
$$\begin{aligned}
TR&=ay-by^2\\
MR&=a-2by
\end{aligned}$$

Now, how try to find $DWL$? Optimal output will be $\hat{y}=\displaystyle\frac{a-c}{b}$, while monopoly's:
$$y^m=\displaystyle\frac{a-c}{2b}$$
So,
$$DWL=\int_{y^m}^{\hat{y}}\left[(a-bt)-c\right]dt=\displaystyle\frac{(a-c)^2}{8b}$$
\end{minipage}%

## The concept of a representative consumer
If an aggregate demand on good can be represented by solving a utility maximization problem of a sole consumer, then we say that in such economy a representative consumer exists. This is exactly the case in a quasilinear economy.

In other words there exists a function $\nu(x)$ such that by solving the problem
\begin{equation}
\begin{cases}
\nu(x)+\sum_{i \in I} z_i \rightarrow \max \\
p \cdot \sum_{i \in I} x_i+\sum_{i \in I} z_i \leq \sum_{i \in I} w_i
\end{cases}
\end{equation}
we can find the aggregate demand function $D(p) =\sum_{i\in I}x_i(p)$