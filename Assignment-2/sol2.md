# Problem-2
## Part-a
For $P$
$$\lVert P(v)-P(u) \rVert \leq \gamma_1\lVert v-u \rVert$$
and for $Q$
$$\lVert Q(v)-Q(u) \rVert \leq \gamma_2\lVert v-u \rVert$$
In the first equation substitute $v$ by $Q(v)$ and $u$ by $Q(u)$. We get,
$$\lVert P(Q(v))-P(Q(u)) \rVert \leq \gamma_1\lVert Q(v)-Q(u) \rVert$$
From the second equation
$$\lVert P(Q(v))-P(Q(u)) \rVert \leq \gamma_1\gamma_2\lVert v-u \rVert$$

$\therefore\, P\circ Q$ is a contraction mapping

Now, there's nothing unique about $P$ or $Q$, we could just swap them and we would still get the same result. Or we would follow the same procedure and get 
$$\lVert Q(P(v))-Q(P(u)) \rVert \leq \gamma_1\gamma_2\lVert v-u \rVert$$

## Part-b
From the solution to above subpart, we can see that the contraction coefficient for both the composite functions is $\gamma_1\gamma_2$ where $\gamma_1$, $\gamma_2$ are the contraction coefficients for $P$ and $Q$ respectively.

## Part-c
The value iteration scheme under the operator would converge to a unqiue solution if it follows
$$\lVert B(v)-B(u)\rVert \leq \lVert v-u\rVert$$
Writing $B$ as a composite function, we can arrive at a general solution with a specific behaviour
$$\lVert F(L(v)) - F(L(u))\rVert \leq \lVert v-u\rVert$$
Assume $\lVert F(v) - F(u)\rVert \leq \eta \lVert v-u\rVert$
Now
$$\lVert F(L(v)) - F(L(u))\rVert \leq \eta\lVert L(v)-L(u)\rVert \leq \eta\gamma \lVert v-u\rVert$$
We get that $\eta < \frac{1}{\gamma}$