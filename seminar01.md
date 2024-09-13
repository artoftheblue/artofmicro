---
abbreviations:
  MC: Marginal Costs
  MR: Marginal Revenue
---

# Seminar 1, 06.09.2024

## Problem 1
The cost function of a non-discriminating monopolist is $c(y) = y^2 + 12$, and the inverse demand function is $p(y) = 24 - y$. 

### Subproblem 1

Find the monopolist's marginal revenue function, equilibrium price and output, and profit. Illustrate graphically the obtained results.

$$\pi=p(y)y-c(y)$$

Revenue function:

$$(24-y)(y)=24y-y^2$$

$$\text{MR}=(24y-y^2)'=-2y+24$$

$$\text{MC}\colon c'(y)=2y$$

$$MC=Mr\colon 2y=-2y+24\iff y^*=6;p^*(y)=18$$

$$\pi =18\cdot6-48=60$$

### Subproblem 2 

Calculate consumer surplus, producer surplus, and the losses (DWL) associated with monopolizing an industry. Illustrate graphically the obtained results. Explain why DWL may occur when an industry is monopolized.

$$\text{CS}=\frac{(24-18)\cdot6}{2}=18$$

$$\text{PS}=\frac{18+6}{2}\cdot 6=72$$

$$\text{DWL}=\frac{6\cdot2}{2}=6$$

### Subproblem 3 

Let the monopolist be taxed in the amount of \$8 from each unit of output. How will the introduction of the tax affect the output of the monopolist, the welfare of consumers and society as a whole? Illustrate graphically.

$$\text{MC}'=\text{MR}'=2y+8=24-2y$$

$$4y=16\implies y=4, p=60$$

$$\text{CS}'=\frac{1}{2}\cdot 4\cdot4=8$$

$$\text{PS}'=\frac{1}{2}\cdot 4(12+4)=8\cdot4=32$$

$$\text{SW}'=\text{CS}'+\text{PS}'+\text{TX}$$

$$\text{DWL}'=\frac{1}{2}\cdot 4\cdot 12 = 24$$

### Subproblem 4

Now let the monopolist be subject to a proportional income tax. How will the introduction of the tax affect the output of the monopolist, the welfare of consumers and society?

$$\pi=(24-y)y-y^2-12$$

$$\pi^{new}=\underbrace{(1-t)((24-y)}_{\text{TR}}y-y^2-12)$$

$$\text{MR}^{new}=((1-t)((24-y)y))'=\text{MR}(1-t)=(1-t)(24-2y)$$

$$\text{MC}=(1-t)2y,\ \text{MR}^{new}=\text{MC}\implies y=6, p=18$$

$$\pi=60(1-t)$$
 
---

Check whether everything is correct (we flunked up somewhere so it's not actually correct):

$$\text{CS}=\frac{(24-18)\cdot6}{2}=18$$

$$\text{PS}=\pi^*=\text{FC}(1-t)=60+12(1-t)$$

$$\text{Taxes}=60t$$

$$\text{SW}=\text{CS}+\text{PS}+\text{Taxes}$$

| | | | |
| --- | --- | --- | --- |
| CS=18 | PS=72  | | DWL=6 |  
| CS'=8 | PS'=32 | Taxes=32 | DWL' = 24 |

$$\text{DWL}=96-90-48t=6-48t$$


## Problem 2

   A monopolist uses technology with a cost function $c(y) = 5/3y^2$ and can sell his product in two regions, price discrimination between which is prohibited. The inverse function of demand for monopoly goods in the first region is $p_1 =10-y_1$, and in the second region $p_2 =13-0.5y_2$.

### Subproblem 1

Find the equilibrium and illustrate it graphically. Will the monopolist sell its product in both regions?

$$y_1=\begin{cases}
    10-p_1, p_1\leq10\\
    0, p>10
\end{cases}$$

$$y_2=\begin{cases}
    26-2p_2,p_1\leq13\\
    0, p>13
\end{cases}
$$

$$y_1+y_2=\begin{cases}
    36-3p,p\leq10\\
    26-2p,p\in(10,13)\\
    0,p>13
\end{cases}$$

$$\pi=\underbrace{p(y)y}_{p\cdot y \, - \,\text{perfect competition}}-c(y)\to\max_{y\geq0}$$

$$p^d=\begin{cases}
    12 - \frac{1}{3}y, \quad 6\leq y\leq 36\\
    13-\frac{1}{2} y, \quad 0\leq y \leq 6
\end{cases}$$

$$\begin{align*}6\leq y\leq 36\colon\, &\pi=12y-\frac{1}{3}y^2-\frac{5}{3}y^2\to\max_y\\&y^*=\frac{12}{4}=3\end{align*}$$

$y^*$ is out of bounds.

$$\begin{align*}0\leq y\leq 6\colon\, &\pi_2=13y-\frac{1}{2}y^2-\frac{5}{3}y^2\to\max_y\\&y^*=\frac{13\cdot6}{13\cdot 2}=3\end{align*}$$

$y^*$ is within bounds.

$$\pi_2=13y-\frac{1}{2}y^2-\frac{5}{3}y^2=13\cdot3-\frac{13}{26}\cdot 3^2=6.5\cdot3=19.5$$

$$\text{CS}=(1.5)^2$$

$$\text{PS}=\pi+0=19.5$$

$$\text{MC}=\frac{10}{3}y$$

### Subproblem 2

Find the DWL of society and illustrate graphically.

# Seminar 2, 13.09.2024

### Subproblem 3 

Now let the monopolist be able to set a different price for his product for two regions, and resale between regions is impossible. Find an equilibrium and illustrate the solution graphically.

---

$$p_1(y_1)=10-y_1$$

$$p_2(y_2)=13-0.5y_2$$

$$c(y)=\frac{5}{3}y^2$$

$$y=y_1+y_2$$

$$\pi(y_1,y_2)=\text{TR}_1(y_1)-c(y)=(10-y_1)y_1+(13-0.5y_2)y_2-\frac{5}{3}(y_1+y_2)^2\to\max_{y_1,y_2\geq0}$$

$$\text{FOC}\colon\begin{cases}\frac{\partial\pi}{\partial y_1}=10-y_1\cdot 2-\frac{5}{3}\cdot2(y_1+y_2)=0\\
\frac{\partial\pi}{\partial y_2}=13-y_2-\frac{10}{3}(y_1+y_2)=0\end{cases}$$

$$\text{SOC}\colon\begin{pmatrix}
    -\frac{16}{3} & -\frac{10}{3}\\
    -\frac{10}{3} & -\frac{13}{3}
\end{pmatrix}$$

$$\Delta_1<0,\quad\Delta 2\colon-\frac{16}{3}\cdot(-\frac{13}{3})-\frac{100}{9}>0$$

$$\begin{cases}
y_1^*=0 & p_1^*\in[10,+\infty)\\
y_2^*=3 & p_2^*=11.5
\end{cases}$$

### Subproblem 4 
 
How will the welfare of consumers, the profit of the monopoly and the total welfare of society change with the possibility of discrimination compared with the equilibrium in the market for a monopoly product in the absence of discrimination? Comment on the result.

Find MR and MC.

---

Everything will be the same

$$\begin{cases}
    p_2^*=11.5\\
    y_1^*=0\\
    y_2^*=3
\end{cases}$$



## Problem 3

The monopolist produces a discrete good at a constant marginal cost of 3. Buyers' reserve prices are shown in the table:

| Quantity | A, Reserve price | B, Reserve price | |
|---------------------------|------------------------------------|-|-| 
| 1                         | 12                                 | 5                |
| 2                         | 5                                  | 4                |
| 3                         | 4                                  | 2                |
| 4                         | 2                                  | 0                |
| 5                         | 0                                  | 0                |

Assuming that there is only one consumer of type $A$ and one consumer of type $B$ in the economy, answer the following questions:

### Subproblem 1
What price will the monopolist set if he cannot discriminate? What profit will he get?

| $p$ | $\pi$ |
| --- | --- |
| $12$ | $12 - 3\cdot1 = 9$ |
| $5$ | $15 - 3\cdot3 = 6$ |
| $4$ | $20 - 3\cdot5 = 5$ |
| $<3$ | $<0$ | 

which implies that $p^*=12,\quad y^*=1$.

### Subproblem 2
What price will the monopolist set if it produces the third-degree price discrimination? What profit will he get?

---

We charge different consumers different prices.

Consider consumer A.

| $p$ | $\pi$ |
| --- | --- |
| $12$ | $12 - 3\cdot1 = 9$ |
| $5$ | $10 - 3\cdot2 = 4$ |
| $4$ | $12 - 3\cdot3 = 3$ |
| $<3$ | $<0$ | 

which implies that $p_A=12,\quad y_A=1$.

Consider consumer B.

| $p$ | $\pi$ |
| --- | --- |
| $5$ | $5 - 3\cdot1 = 2$ |
| $4$ | $8 - 3\cdot2 = 2$ |
| $4+\varepsilon$ | $(4+\varepsilon)\cdot1-3\cdot1=1+\varepsilon$ |
| $<3$ | $<0$ | 

Total optimal profit then would be $\pi^*=11-9$

### Subproblem 3
Assuming that the monopolist can use the first-degree price discrimination, find the prices for each unit sold, the monopolist's output, and the profit.

### Subproblem 4
Compare the profit in points (1), (2), (3) and explain the result.

---

We may set any price for any separate unit that we sell. In this case, we iteratively set the price for each of the units first to $12$, then to $5$, and then $4$.

$$\pi_A=\underbrace{(12-3)}_{\pi_{1A}}+(5-3)+(4-3)=12$$

$$\pi_B=(5-3)+(4-3)=3$$

$$\pi^*=15>11>9$$

The first type of discrimination has a higher profit than the third one and even higher than the monopoly case.

$$\pi_{1^{\text{st}}}\geq\pi_{3^{\text{rd}}}\geq\pi_m$$

### Subproblem 5

Show how the first-degree price discrimination result could be achieved:  
1. through a two-stage payment (linear price plus access fee),
2. through a bundle sale.

---

$$A_i+p_i\cdot q_i$$

We could set any price and any access fee, but the easiest way to collect all the money that the consumer is willing to price is to set the price equal to marginal cost (MC) & set the access fee to the total of markups.

$$p_i=3,A_A=12, A_B=3$$

$$\pi_A=A_A+(P_A-3)\cdot \underbrace{q_A}_{q_A(p_A,A_A)}\to\max_{A_A,p_A\geq0}$$

Alternatively, we could

$$p_A=4,A_A=9\implies \pi=12$$

The consumer get a total surplus of $9=A_A$


## Problem 4

Consider two groups of consumers. The consumers of group $H$ are represented by an aggregated consumer with a demand function for goods $y$ of the form $y^H =4-p$, and the demand of an aggregated consumer of group $L$ has the form: $y^L =3-p$. We will assume that the number of consumers in the groups is the same. Good $y$ is produced by a monopoly firm using constant returns to scale technology. The marginal cost of producing good $y$ is constant and equal to 1.

### Subproblem 1
Assuming that the monopolist is able to prevent the resale of the product, find for each group the optimal two-stage payment scheme for the product (fee for the right to purchase the product plus the linear price).

---

Most simple way, just set price to MC. Then we would get 

$$p_h=p_l=1$$

$$A_h=\frac{3\cdot 3}{2}=4.5$$

$$A_l=\frac{2\cdot 2}{2}=2$$

$$\pi=A_h+A_l=2+4.5=6.5$$

More formally,

$$CS_l=\frac{(3-p(q_l))\cdot q_l}{2}=\frac{(3-3+q_l)q_l}{2}=\frac{q_l^2}{2}=A_l$$

$$CS_h=\frac{q_h^2}{2}$$

$$\pi=\frac{q_l^2}{2}+\frac{q_h^2}{2}+(3-q_l)q_l+(4-q_h)q_h-3(q_l+q_h)\to\max_{q_k,q_h}$$

$$p_l=q_h=1, \pi^*=6.5$$

### Subproblem 2

Find the optimal two-component tariff, assuming that the tariff should be the same for both regions.

---

$$A+p\cdot y_i$$

Firstly, we try to sell our product only to $H$.

$$A=4.5,\quad p=1,\quad\pi^*=4.5$$

Secondly, 

$$A=\frac{p_l^2}{2}$$

$$p=3-q+l$$

$$y_l=q_l$$

$$y_h=4-\underbrace{(3-q_l)}_p=1+q_l$$

$$\pi=2\cdot\frac{q_l^2}{2}+(3-q_l)(q_l+1+q_l)-(q_l+1+q_l)\max\to q_l>0$$

$$\pi^*=4.25$$

### Subproblem 3 

How will a monopolist behave if it can offer two two-component tariffs, but each consumer chooses which tariff to subscribe to?

### Subproblem 4

Solve the problem under the assumption that there are twice as many consumers in group $L$ as in group $H$.