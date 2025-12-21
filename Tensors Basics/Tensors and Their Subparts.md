


# I - Tensors Basics

## 1 - Tensors and Their Subparts

### 1.1 - What is a Tensor?

> **Definition (Tensor):**<br>
> A Tensor is a *d*-way array, where *d* is referred to as the **order** of the tensor.

We can say that a Tensor of oder 1 is a Vector, a Tensor of order 2 is a Matrix, etc
```
   +----+			    +--------------------+
   | x1 |	    		| x(1,1) ..    x(1,n)|
   | x2 |               | ..                 |
   | .. |               |                    |
   | xn |               | x(m,1)       x(n,m)|
   +----+               +--------------------+
   a) x                          b) x          
   ```                       
*a)*		A vector $\mathbf{x} \in \mathbb{R}^n$ is a tensor of order $1$. <br>
*b)*  	A matrix $\mathbf{x} \in \mathbb{R}^{m\times n}$ is a tensor of order $2$.

Furthermore, a Tensor of order 3 can be seen as an array of Tensor of order 2, a Tensor of order 4 can be seen as an array of Tensor of order 3, and so on.

> **Definition (Higer Order):** <br>
> A *d*-way tensor is called **higher order** if *d* ≥ 3.

Let's take a Tensor of order 3 denoted as $\mathbf{X} \in \mathbb{R}^{m\times n \times p}$, we refer each dimension as a **mode**:
		     -      **mode 1** is of size *m*
			 -      **mode 2** is of size *n*
			 -      **mode 3** is of size *p*
More generally, for each mode $k \in \{1,\dots,d\}$, its size is denoted by $n_k$.
And if all modes share the same size, we call the tensor **cubical**.

> **Exercise 1.1** – How many entries are in a tensor of size $\text{100} \times \text{80} \times \text{60}$?

<details>
<summary>Show answer</summary>

The total number of entries in a tensor is the product of its dimensions,  
so $\text{100} \times \text{80} \times \text{60} = \text{480 000 entries}$.

</details>

>**Exercice 1.2** - (a) Consider a 3-way tensor of size $\text{512} \times \text{512} \times \text{512}$. If each entry is a double precision value that requires 8 bytes of memory, how many gigabytes of memory are need for a tensor *(note that a gigabyte is $2^{30}$ bytes).* (b) What about a 4-way tensor of size  $\text{512} \times \text{512} \times \text{512} \times \text{512}$?

