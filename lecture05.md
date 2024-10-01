# Lecture 5, 01.10.2024

## Cooperative behaviour of firms

In order to improve profitability, the firms have to reduce their outputs. It is clear from the figure below where the arrow shows the direction output reduction where the profits go up.

```{figure} ./image-24.png
:height: 300
:label: lecture5-1
The arrow shows the direction of output reduction.
```

Similarly, let's suppose we have Cournot's duopoly.

Then, their profits are 

$$\pi_1=p(y_1+y_2)y_1-c_1(y_1)$$

and

$$\pi_2=p(y_1+y_2)y_2-c_2(y_2)$$

Let $dy_i<0, dy_w=0$ using total differentials we get at $(y_1^C, y_2^C)$.

$$d\pi_1=p(y_1+y_2)dy_1+y_1p'(y_1+y_2)(dy_1+dy_2)-c'_1(y_1)dy_1\bigm|_{dy_2=0}=\\ = dy_1(p(y_1+y_2)+p'(y_1+y_2)y_2-c_1'(y_1))=0$$

at $(y_1^C,y_2^C).

At the same time,

$$d\pi_2=y_2p'(y_1+y_2)dy_1>0$$

If $n\leq 3$ and at least 2 of them decide to cut the outputs then we have improvement for all firms.

We say that the firms collude if agree about their outputs after bargaining, setting production quotas.

Each point in the bargaining set is a collusion point between the firms.

In other words, a collusion point $(\tilde y_1,\tilde y_2,\ldots,y-\tilde y_n)$ satisfies conditions:

1. $\pi_j(\tilde y)\leq\pi_j(y^C)$ for $j=\overline{1, n}$;
2. $\tilde y$ is Pareto optimal.

Here $y^C=(y_1^C,y_2^C,\ldots,y_n^C)$ is Cournot's equilibirium over which the firms start to negotiate.

## Cartel 

```{prf:definition}
**Cartel** is a form of cooperation when the firms-participants in the cartel share their profits.

That means that they maximize the total profit 

$$\sum^n_{j=1}\pi_j=p(Y)Y-\sum^n_{j=1}c_j(y_j)\xrightarrow[y_1,y_2,\ldots,y_n]{}\max$$
```

In other words, a cartal is a monopoly with $n$ plants.

It's interesting that a cartel may include advanced technology as well as backward firms.

The FOC for cartel maximization is 

$$p(Y^k)+p'(Y^k)Y^k\leq c'_j(y_j^k)$$

and

$$p(Y^k)+p'(Y^k)Y^k=c_j'(y_j^k)$$

if $y_j^k>0$

```{prf:example}
Given $MC_1=c_1<MC_2=c_2$, the outputs in case of a linear demand would be 

$$y_1^k=\frac{a-c_1}{2b}$$

and

$$y_2^k=0$$
```

The next proposition tells us that a cartel is unstable.

```{prf:proposition}
Let $y_j^k>0$ for $j=\overline{1,n}, c_j(y_j)\in C^1, p(Y)
\in C^1$ and $p'(Y)<0$ for $Y>0$. Then

$$\frac{\partial\pi_j}{\partial y_j}\biggm|_{Y^k}>0,\forall j=\overline{1, n}$$

In other words, cartel memebers would prefer to increase their outputs in the violation of their agreement.
```

## Problem 6

$n$ identical firms face $Y=1-p$ demands. Firms have $MC_i=0$ and compete by choosing outputs.

### Subproblem A

Let firms number $n +1$ be planning to enter the market. To enter it, one has to pay $F$ dollars for the license and if so, it will join the market and compete for the Cournot equilibirium. Find $F_{\max}$ that still allows a firm to enter.

---

$$p=1-Y=1-\sum^{n+1}_{j=1}y_j$$

$$\pi_i=(1-\sum^{n+1}_{j=1})y_i$$

$$\frac{\partial \pi_i}{\partial y_i}=1-\sum^{n+1}_{j=1}y_j-y_i=0$$

$$y_i=y^*>0$$

$$1-(n+2)y^*=0,\quad y^=\frac{1}{n+2}$$

$$y^*=\frac{n+1}{n+2},\quad p^*=1-\frac{n+1}{n+2}=\frac{1}{n+2}$$

$$\pi^*_{n+1}\geq F$$

$$\pi^*_{n+1}=\frac{1}{(n+2)^2}\leq F$$

$$\boxed{F_{max}=\frac{1}{(n+2)^2}}$$

### Subproblem B

The decides not to enter and this time these $n$ firms organized a cartel. The cartel offers the entrant a two-stage game. Firstly, the cartel chooses its output $y_k$, then the entrant decides whether to enter the market or not. If it decides to enter, it chooses the output and at this stage the proce is set. Find how the profit of the entrant depends on $y_k$ and $F$.

---

$$\pi_{n+1}=(1-y_k-y_{n+1})y_{n+1}\to\max_{y_{n+1}\geq 0}$$

$$\frac{\partial\pi_{n+1}}{\partial y_{n+1}}=1-y_k-2y_{n+1}=0$$

$$y_{n+1}=\frac{1-y_k}{2}$$

$$\pi_{n+1}=\frac{1-y_k}{2}\cdot\frac{1-y_k}{2}=\left(\frac{1-y_k}{2}\right)^2\geq F$$

When a firm doesn't enter?

$$\left(\frac{1-y^k}{2}\right)^2-F\leq 0$$

$$(1-y_k)^2\leq F\leq F\cdot 4$$

$$1-y_k\leq 2\sqrt{F}$$

$$\boxed{y_k\geq 1-2\sqrt{F}}$$

---

$$\pi_k=(1-y_k)y_k\to\max$$

$$\boxed{y_k=\frac{1}{2}}$$

Now we'll be considering several scenarios.

### Subproblem C

Suppose $F$ is at $F_{max}$ level and we learned that the firm did not enter. What can be said about it?

---

#### Scenario 1 

The cartel decides to stop entering by choosing the biggest output it can afford in terms of profitability. Then $\frac{1}{4}$ would be the profit value.

$$\boxed{\underset{1/2}{y_k}\geq 1-2\underset{=\frac{1}{(n+2)^2}}{\sqrt{F}}}$$

$$\frac{1}{2}\geq 1-\frac{2}{n+2}$$

$$\frac{2}{n+2}\geq \frac{1}{2},\quad n+2\leq 4\implies n=2$$

this means that there should be two firms on the market for the cartel not to let any new firm to the market.

#### Scenario 2

$$y_{n+1}=\frac{1-y_k}{2}$$

$$\pi_k=(1-y_k-y_{n+1})y_k$$

$$\left[\left(\frac{1-y_k}{2}\right)y_k\right]'=0$$

$$y_k=\frac{1}{2}$$

$$y_{n+1}=\frac{1}{4}$$

$$\pi_k=\left(1-\frac{1}{2}-\frac{1}{4}\right)\frac{1}{2}=\frac{1}{8}$$

Let's find all possible values of $y_k$

$$y_k=1-\frac{2}{n+2}=\frac{n}{n+2}$$

Cartel fears the increasing the amount of production may negatively influence its profit, let's check this:

$$\left(1-\frac{n}{n+2}\right)\frac{n}{n+2}=\frac{2n}{(n+2)^2}>\frac{1}{8}$$

solving the inequation above, we get

$$\boxed{3\leq n\leq 11}$$

Thus it is beneficial for the cartel to increase output, so the firm would not profit from entering the market.

## Bertrand's model

We consider $n$ firms with $MC_i=c>0$, $i=\overline{1,n}$. The demand is given by $y=D(p)$, where $D'(p)<0$ for $y>0$.

...

Let $y_i$ denote the demand for the $i$-th firm output. Then $y_j=D_j(p_j,\overline{p_{-j}})$. The following conditions should be met:

1. let $p_{i_0}>\max\{p_1,p_2,\dots,p_n\}$, then $y_{i0}=0$ (this good is too expensive)
2. let $k$ firms set the same minimum price, then the rest of the firms can not sell, and the supply provided by each of these $k$ firms will be equal
3. fixed costs are zero.

Then the Bertrand-Nash equilibirum satisfies the following theorem:

```{prf:theorem}
The equilibirum establishes itself on $p_{\min}=c$ and it will be supported by at least two firms from oligopoly. **Bertrand's paradox has an explanation.**
```

```{prf:proof}
$\exists a$ firm setting $p_{\min}>c$

$\exists$ some other firm chooses $p_{\min}-\varepsilon>c$

$D(p_{\min})=0$

$D(p_{\min}-\varepsilon)>0$

Let's assume the contrary, that the minimum price is chosen by one firm only. Then, if other firms do not sell it at all, then the firm can add epsilon to $c$ value, and epsilon may be small enough to be smaller than all other prices and thus everyone would buy at this price.

> Sorry the explanation was not written out anywhere so it's kinda weird.

Thus we get a contradiction because it's only possible for the minimums for each firm to be syncronized.

There is a problem that this is a one-shot simultaneous game, which isn't applicable to the real world since firms compete in prices long-term.
```

The model is oversimplistic

1. should be dynamic, accounting for many stages;
2. firms are not necessarily the same and $MC_i$ can be variable;
3. the product may be differentiated (close substitutes).

Within out course of micro, we consider what happens if we allow the firms (like in Bertrand's model) to interact many times, or infinitely many times.

### Stream of profits

$$\Pi_1=\sum^\infty_{t=1}\delta^{t-1}\cdot\frac{\pi^m}{2}=\frac{\pi^m}{2}\cdot\frac{1}{1-\delta}$$

$$\Pi_2=\frac{\pi^m}{2}\cdot\frac{1}{1-\delta}$$

where $\pi^m$ is monopoly profit. 

```{note}
<wiki:Tacit_collusion> is a collusion between competitors who do not explicitly exchange information but achieve an agreement about coordination of conduct. 
```

```{prf:theorem}
In the setting of the Bertrand's model $p_{jt}=p^m$ if and only if $\delta\geq\frac{1}{2}$.
```

```{prf:proof}
$$\frac{\pi^m}{2}\cdot\frac{1}{1-\delta}\geq\pi_m-\cancel\varepsilon$$

$$\frac{1}{2}\cdot\frac{1}{1-\delta}\geq 1$$

$$\frac{1}{1-\delta}\geq 2$$

$$1-\delta\leq\frac{1}{2}$$

$$\delta\geq \frac{1}{2}$$
```

## Price leadership

This is a sequential two stage model where there is a leader that sets the price and other firms-followers sometimes called "competitive fringe"m because they take this proce as given. The solution is done in backward fashion. At stage 2 $j$-th firm ($j$ ranges from $2$ from $n$) solve a problem of choosingthe profit maximizing output when 


$$py_j-c_j(y_j)\xrightarrow[y_j\geq 0]{}\max$$

$j$-th firm from the "fringe"

$$py_j-c_j(y_i)\to\max_{y_j\geq 0}$$

best response function 

$$y_j=s_j(p)=\boxed{p=c'_j(y_j)}$$

Let $y_j(p)$ be a solution of this maximization. Then, the leader will face the residual demand

$$D_1(p)=D(p)-\sum^n_{j=2}y_j$$

Following backwards induction, the leader behaves as a monopoly by solving 

$$\pi_1=pD_1(p)-c_1(D_1(p))\xrightarrow[p]{}\max$$

[add picture later]

```{figure} ./
Here you can find 2 figures illustrating how the equilibrium price should be found.
```

## Choice under uncertainty

### Axiomatic approach

Let $A=\{a_1,a_2,\dots,a_n\}$ denote the finite set of outcomes. A simple gamble assigns a probability $p_i$ to each of the outcomes $a_i\in A$.

Clearly, $p_i\geq 0$ and $\displaystyle\sum_ip_i=1$

The gamble must result in some outcome of $A$. We denote $g=(p_1\circ a_1,p_2\circ a_2,\ldots,p_n\circ a_n)$

The set of all simple gambles is $G_S$.

But the outcomes can be gambles themselves. Then they are called compound.

We assume that such compound gambles will finally result in some outcome from $A$ after some randomizations.

We keep the same notations for the preferences:

1. $\succeq$ no worse than
2. $\succ$ better than
3. $\sim$ same as

Consider the set $G$ of all gambles, simple and compound.

```{prf:axiom} G1. Completeness
For any two gambles $g$ and $g'$ in $G$, either $g'\succeq g$ or $g\succeq g'$.
```

```{prf:axiom} G2. Transitivity

For any three gambles $g, g', g''$ in $G$ if $g\succeq g'$ and $g'\succeq g''$, then $g\succeq g''$
```

```{prf:axiom} G3. Continuity

For any $g$ in $G$ there exists some probability $\alpha\in[0, 1]$ such that $g\sim(\alpha\circ a_1, (1-\alpha)\circ a_n)$, where $a_1$ is the best outcome and $a_n$ is the worst outcome.
```

```{prf:axiom} G4. Monotonicity
For all probabilities $\alpha, \beta\in[0, 1]$,

$$(\alpha\circ a_1,(1-\alpha)\circ a_n)\succeq(\beta\circ a_1,(1-\beta)\circ a_n) \iff \alpha\geq\beta$$
```

```{prf:axiom} G5. Substitution
If $g=(p_1\circ g_1\ldots p_k\circ g_k)$ and $h=(p_1\circ h_1\dots,p_k\circ h_k)$, given $g_i\sim h_i$ for every $i$, then $g\sim h$.
```

```{prf:axiom} G6. Reduction to simple gambles
For any $g\in G$ there exist the probabilities $p_i, i\in\overline{1, n}$ that $g\sim(p_1\circ a_1,\ldots, p_n\circ a_n)$.
```

$$g_1=(p\circ a_1,(1-p)\circ g_2), \quad\text{simple}$$
$$g_2=(q\circ a_1,(1-q)\circ a_2),\quad \text{compound}$$
$$\tilde p=p+(1-p)q,\quad \tilde q=(1-p)(1-q)=1-\tilde p$$
$$g_1\sim(\tilde p\circ a_1)$$

```{prf:definition}
The utility function $U(g)\colon G\to\mathbb{R}$ has the expected utility property if, for every $g\in G, U(g)=\displaystyle\sum^n_{i=1}p_iU(a_i)$, where $g\sim(p_1\circ a_1,\ldots, p_n\circ a_n)$.
```

```{prf:remark}
Such simply gamble $(p_1\circ a_1,\ldots, p_n\circ a_n)$ that is indifferent with $g$ is called **induced** by $g$.

$U(g)$ with the expected utility property is also called VNM utility function referring to John von Neumann.
```

```{prf:theorem} Theorem of existence of VNM function on G.
Let preferences $\succeq$ over gambles in $G$ satisfy all $6$ axioms from $G1$ to $G6$. Then there exists a utility function $U(g)\colon G\mapsto\mathbb{R}$ representing preference $\succeq$ on $G$ that VNM function.
```

We remember from utility maximization theory that a utility function is not unique. 

$$\begin{cases}
    U(x,y)=x^\alpha y^\beta\\
    p_xx+p_yy=I\\
    MRS_{xy}=\frac{p_x}{p_y}
\end{cases}$$

$$U(x,y)=\alpha \ln x \beta \ln y$$

What about $VNM$ functions?

```{prf:theorem}
VNM functions are unique up to positive linear transformations. In other words, if $U(g)$ represents $\succeq$ preference, then the VNM function $\nu(g)$ represents the same preference if there exists $\alpha$ and $\beta>0$ such that $\nu(g)=\alpha+\beta U(g)$.
```

### Risk aversion

From now we consider only money outcomes.

Then, simple gamble looks like $g=(p_1\circ w_1,\ldots,p_n\circ w_n)$ where $p_i$ is a probability of receiving $w_i\in\R$.

Let us compare $U(g)$ that is given by $U(g)=\displaystyle\sum^n_{i=1}p_iU(w_i)$ with the utility value of receiving expected outcome $\mathbb{E}g=\displaystyle\sum^n_{i=1}p_iw_i$ with certainty.

Let $g=(p_1\circ w_1,\ldots,p_n\circ w_n)$.

If $U(\mathbb{E}g)>U(g)$, we say an individual is risk-averse for $g$.

If $U(\mathbb{R}g)<U(g)$, we say an individual is risk-loving.

If $U(\mathbb{E}g)<U(g)$, we say an individual is risk-neutral.

If the same inequalities hold for every $g\in G$, we classify this individual using the same names, but globally (i. e. on $G$).

---

Elementary utility functions 

$$U(W)=W^\alpha,\quad 0<\alpha< 1$$

Bernoullian utility

$$u(g)=Eu=p(w_1)^\alpha+(1-p)(w_2)^\alpha$$

$$Ew=pw_1+(1-p)w_2$$

$$0<p<1,\quad u(Ew)>Eu$$

```{figure} ./image-25.png
:height: 300
```

```{figure} ./image-26.png
:height: 400
```

```{figure} ./insert-lecture-picture.png
insert-lecture-picture.png
```

```{prf:definition}
The certainty equivalent $CE$ of any simple game over wealth levels is an amount of wealth offered with certainty such that 
$$U(g)\equiv U(CE)$$
```

```{prf:definition}
The risk premium is an amount of wealth $P$ such that $U(g)=U(\mathbb{E} g-P)$ or $P=\mathbb{E}g-CE$.
```

```{prf:definition}
The Arrow-Pratt measure of absolute risk-aversion is given by 

$$R_a(w)=-\frac{U''(w)}{U'(w)}$$
```

```{prf:theorem}
Two risk-averse individuals have $U(g)$ and $\nu(g)$ VNM functions, respectively.

Let their Arrow-Pratt measures $R_a^1(w)>R^2_a(w),\forall w\geq0$, where

$$R^1_a(w)=\frac{U''(w)}{U'(w)}$$

and

$$R^2_a(w)=\frac{\nu''(w)}{\nu'(w)}$$

Then there exists $C^2$ function $h(x)$ with $h''(x)<0$ for $x>0$ such that $U(w)=h(\nu(w))$.

Furthermore,

$CE_1<CE_2$ where $CE_1$ and $CE_2$ are their respective certainty equivalents.
```
