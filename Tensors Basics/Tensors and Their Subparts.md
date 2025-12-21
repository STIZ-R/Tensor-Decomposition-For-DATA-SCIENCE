


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

Let's take a Tensor of order 3 denoted as $\mathbf{X} \in \mathbb{R}^{m\times n \times p}$, we refer each dimension as a **mode**: <br>
		     -      **mode 1** is of size *m* <br>
			 -      **mode 2** is of size *n* <br>
			 -      **mode 3** is of size *p* <br><br>
More generally, for each mode $k \in \{1,\dots,d\}$, its size is denoted by $n_k$. <br>
And if all modes share the same size, we call the tensor **cubical**. <br> <br>

> **Exercise 1.1** – How many entries are in a tensor of size $\text{100} \times \text{80} \times \text{60}$?

<details>
<summary>Show answer</summary>

The total number of entries in a tensor is the product of its dimensions,  
so $\text{100} \times \text{80} \times \text{60} = \text{**480 000 entries**}$.

</details>
<br>

> **Exercise 1.2** –  
> (a) Consider a 3-way tensor of size $\text{512} \times \text{512} \times \text{512}$.  
> If each entry is a double precision value that requires 8 bytes of memory, how many gigabytes of memory are needed for the tensor (note that a gigabyte is $2^{30}$ bytes)?  
> (b) What about a 4-way tensor of size $\text{512} \times \text{512} \times \text{512} \times \text{512}$?

<details>
<summary>Show answer</summary>

For the 3-way tensor, the number of entries is $512^3 = 134{,}217{,}728$,  
so the total memory is $134{,}217{,}728 \times 8 \approx 1.07 \times 10^9$ bytes, i.e., **1 GB**.  

For the 4-way tensor, the number of entries is $512^4 = 68{,}719{,}476{,}736$,  
so the total memory is $68{,}719{,}476{,}736 \times 8 \approx 5.50 \times 10^{11}$ bytes, i.e., **512 GB**.

</details>


