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

| --- | --- | --- | --- |
| CS=18 | PS=72  | | DWL=6 |  
| CS'=8 | PS'=32 | Taxes=32 | DWL' = 24|

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


### Subproblem 3 

Now let the monopolist be able to set a different price for his product for two regions, and resale between regions is impossible. Find an equilibrium and illustrate the solution graphically.

### Subproblem 4 
 
How will the welfare of consumers, the profit of the monopoly and the total welfare of society change with the possibility of discrimination compared with the equilibrium in the market for a monopoly product in the absence of discrimination? Comment on the result.
