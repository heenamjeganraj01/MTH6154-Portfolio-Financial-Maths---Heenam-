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

The symbol 
