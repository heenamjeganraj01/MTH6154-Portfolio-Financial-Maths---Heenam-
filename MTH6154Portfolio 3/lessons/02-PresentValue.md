# 2. Present Value and Rates of Return

[Back to contents](../README.md)

## Summary

### Present Value Analysis

#### Present Value

**Present value** tells us how much money received in the future is worth today. Money received today can earn interest, so future payments must be discounted to compare their values fairly. 

Let $V$ be the future payment, $r$ the effective annual interest rate and $t$ the number of years. 

$$
PV(V)=\frac{V}{(1+r)^t}=V(1+r)^{-t}
$$

If interest is compounded $n$ times per year at nominal annual rate $r$, the formula becomes: 

$$
PV(V)=V\left(1+\frac{r}{n}\right)^{-nt}
$$

#### Cash-Flow Streams

A cash-flow stream is a series of payments received or paid at different times: 

$$ 
a=(a_1,a_2,\ldots,a_n)
$$

Here, $a_i$ is the payment at the end of year $i$. To find the total present value, we discount each payment and add them together: 

$$
PV(a)=\sum_{i=1}^{n}\frac{a_i}{(1+r)^i}
$$

The symbol $\sum$ means adding all the terms. Two investments that produce exactly the same future payments have the same **present value**. This is called **replication**. 

#### Perpetuities

A perpetuity is an investment that pays the same amount every year forever. 

The geometric-series formula is: 

$$
\sum_{i=0}^{n}x^i=\frac{1-x^{n+1}}{1-x}
$$

For $|x|<1$, the infinite series becomes: 

$$
\sum_{i=0}^{\infty}x^i=\frac{1}{1-x}
$$

Using the result, the present value of a perpetuity paying $a$ each year is: 

$$
PV(a)=\sum_{i=1}^{\infty}\frac{a}{(1+r)^i}=\frac{a}{r}
$$

This assumes interest is: $r>0$, and payments begin after one year. 

#### Discount Factors

A ,**discount factor**, $D(T)$, tells us how much £1 received in $T$ years is worth today. 

For annual compounding: 

$$
D(T)=\frac{1}{(1+r)^T}
$$

If interest is compounded $n$ times per year: 

$$
D(T)=\left(1+\frac{r}{n}\right)^{-nT}
$$

For continuous compounding at a constant rate: 

$$
D(T)=e^{-rT}
$$

For a changing instantaneous interest rate, covered in lesson 1, using the **yield curve** $\bar r(T)$ also from Week 1:

$$
D(T)=e^{-T\bar r(T)}
$$

Discount factors allow us to calculate the present value of payments $a_i$ made at times $t_i$:

$$
PV=\sum_{i=1}^{n}D(t_i)a_i
$$

A smaller discount factor means future money is worth less today. 

#### Balancing Present Values

When planning savings of future payments, the present value of money going in must equal the present value of money coming out to ensure net zero value: 

$$
PV(\text{deposits})=PV(\text{withdrawals})
$$

For example, someone saving for retirement can use this equation to find out how much they need to deposit each month to cover future withdrawals. 

We can also compare 
