# Seminar 4, 27.09.2024

## Cournot and Stackelberg Oligopoly Models

### Problem 1

There are only two firms in the industry. The cost funciton of firm A is $c_1(y_1)=0.5y_1$ and the cost function of firm B is $c_2(y_2)=1.5y_2$. The demand is $p(y)=2-y$, where $y=y_1+y_2$. Two firms choose $y_i$ simultaneously.

1. Find the Cournot equilibrium.

2. Find the Cournot equilibirium when $c_1(y_1)=y_2^2$ and $c_2(y_2)=2y_2^2$.

---

$$\left.\begin{align*}c_1=0.5y_1\\ c_2=1.5y_2\end{align*}\right\}\implies c_i=a_iy_i$$

$$a_i\in\{0.5, 1.5\}$$

$$p(y)=2-y$$

$$y=y_1+y_2$$

$$\pi_i=p(y)y_i-c_i(y_1)\to\max_{y_1\geq 0}$$

$$\pi_i=(2-y_1-y_2)y_i-a_iy_i\to\max_{y_i\geq 0}$$

$$\pi_1=(2-y_1-y_2)y_1-0.5y_1\to\max_{y_1\geq 0}$$

$$\frac{\partial\pi}{\partial y}=2-2y_1-y_2-0.5=0$$

Thus, the best responce for the first person would be:

$$BR_1\colon \textcolor{purple}{y_1}=\begin{cases}\displaystyle\frac{1.5-y_2}{2}, & y_2\leq 1.5\\
0, & \text{otherwise}\end{cases}$$

$$BR_2\colon \textcolor{green}{y_2}=\begin{cases}\displaystyle\frac{0.5-y_2}{2}, & y_2\leq 0.5\\
0, & \text{otherwise}\end{cases}$$

$$NE\colon \begin{align*}y_1^*=0.75\\ y_2^*=0\end{align*}$$

$$y_1=1\implies y_2(1)=0\implies y_1(0)\implies 0.75\implies y_2(0.75)=0\implies NE$$

```{figure} ./image-21.png
:label: sem04-1
Graph visualization 
```

$$y_1=0.25\implies y_2(0.25)=0.125\implies y_1(0.125)=\frac{1.375}{2}\implies y_2(0.6875)=0\implies y_1(0)=0.75$$

---


```{figure} ./image-22.png
:label: sem04-2
Graph visualization-2
```

$$y_i=\frac{a-c_i-y_i}{2}$$

$$c_1=c_2$$

### Problem 2

There are only two firms in the industry. The cost function of each firm is $c_i(y_i)=2y_i$, where $i\in\{1,2\}$. The demand function is $y=8-p$. Suppose that the first firm (leader) decides how much to produce, and the the second firm (follower) makes a decision about the output, considering the choice of the first firm as given.

#### Subproblem 1

Find the equilibrium outputs of each firm.

---

$$\pi_2=(8-y_1-y_2)y_2-2y_2\to\max_{y_2\geq 0}$$

$$\pi_2=(6-\underset{=6-y_1}{y_1}-\overset{=0}{y_2})y_2\to\max_{y_2\geq 0}$$

$$y_2^*=\begin{cases}\displaystyle\frac{6-y_1}{2}, & y_1\leq 6\\
0, & \text{otherwise}\end{cases}$$

$$\pi_1=(8-y_1-y_2(y_1))y_1-2y_1\to\max_{y_1\geq 0}$$

$$\pi_1=\begin{cases}(8-y_1-\frac{6-y_1}{2}-2)y_1, & y_1\leq 6\\
(8-y_1-0-2)y_1, & \text{otherwise}\end{cases}\to\max_{y_1\geq 0}$$

$$\pi=\begin{cases}
    \displaystyle\left(\frac{6-y_1}{2}\right)y_1, & y\leq 6\\
    (6-y_1)y_1, & y > 6
\end{cases}\to\max_{y_1\geq 0}$$

$$y_1^*=3,\quad pi_1^*=4.5>0$$

$$y_2^*=\begin{cases}
    \displaystyle\frac{6-y_1}{2}, & y\geq 6\\
    0, & \text{otherwise}
\end{cases}$$

$$p=8-3-1.5=3.5$$

$$\pi_2^*=$$

$$\pi_2=(6-\underset{=6-y_1}{y_1}-\overset{=0}{y_2})y_2\to\max_{y_2\geq 0}$$

$$BR_2\colon y_2^*=\begin{cases}\displaystyle\frac{6-y_1}{2}, & y_1\leq 6\\
0, & \text{otherwise}\end{cases}$$

$$BR_1\colon y_1^*=\begin{cases}
    \frac{6-y_2}{2}, & y_2\leq 6\\
    0, & \text{otherwise}
\end{cases}$$

$$y_2=\frac{6-\frac{6-y_2}{2}}{2}\implies 4y_2=12-6+y_2$$

$$\begin{align*}
    y_1^*=2\\
    y_2^*=2\\
    \pi^*_1=\pi^*_2=4
\end{align*}$$

## Price Competition

### Problem 10. Bertrand Equilibirum

#### Subproblem 1

$$N=2\quad c_1=c_2$$

$$\pi_1=\begin{cases}
    0, & p_1 > p_2\\
    \frac{1}{2}(p_1-c_1)(a-p_1), & p_1=p_2\\
    p_1y_1-c_1y_1, & p_1<p_2
\end{cases}$$

$$BR_1\colon p_1=\begin{cases}
    p_2-\varepsilon, & p_2>c_1\\
    c_1, & p_2\leq c_1
\end{cases}\in(p_2,+\infty)$$

```{figure} ./image-23.png
:label: fig-23
Graphical visualization
```

$$BR_2\colon p_2=\begin{cases}
    p_1-\varepsilon, 
\end{cases}$$

---

$$p_1=p_2=c_1=c_2$$

2.