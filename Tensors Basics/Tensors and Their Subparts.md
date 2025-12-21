

# I - Tensors Basics

## 1 - Tensors and Their Subparts

### 1.1 - What is a Tensor?

> **Definition (Tensor):**
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
a)		A vector $\mathbf{x} \in \mathbb{R}^n$ is a tensor of order $1$.
b)  	A matrix $\mathbf{x} \in \mathbb{R}^{m*n}$ is a tensor of order $2$.

Furthermore, a Tensor of order 3 can be seen as an array of Tensor of order 2, a Tensor of order 4 can be seen as an array of Tensor of order 3, and so on.

> **Definition (Higer Order):**
> A *d*-way tensor is called **higher order** if *d* ≥ 3.

Let's take a Tensor of order 3 denoted as $\mathbf{X} \in \mathbb{R}^{m*n*p}$, we refer each dimension as a **mode**:
		     -      **mode 1** is of size *m*
			 -      **mode 2** is of size *n*
			 -      **mode 3** is of size *p*
