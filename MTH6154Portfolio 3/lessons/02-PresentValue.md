# 2. Present Value and Rates of Return

[Back to contents](../README.md)

## Summary

### Present Value Analysis

#### Present Value

**Present value** tells us how much money received in the future is worth today. Money received today can earn interest, so future payments must be **discounted** to compare their values fairly. 

Let $V$ be the future payment, $r$ the effective annual interest rate and $t$ the number of years. 

$$
PV(V)=\frac{V}{(1+r)^t}=V(1+r)^{-t}
$$

If interest is compounded $n$ times per year at nominal annual rate $r$, the formula becomes: 

$$
PV(V)=V\left(1+\frac{r}{n}\right)^{-nt}
$$

#### Net Present Value (NPV)

Net Present Value (NPV) tells us whether an investment is worth making by comparing the **present value** of money received with money paid out. 

On a cash-flow timeline, upward arrows represent money received, while downward means money gone out. 

For an initial investment $P$ and future payments $a_i$ received at the end of year $i$ is: 

$$
NPV=-P+\sum_{i=1}^{n}\frac{a_i}{(1+r)^i}
$$

Here, $r$ is the **effective annual rate** and $n$ is the number of years: 

- **NPV > 0** The investment is financially worthwhile at the chosen interest rate
- **NPV<0** The investment is not financially worthwhile at the chosen interest rate
- **NPV = 0** The investment does not gain profit and earns enough to cover its cost

A higher interest rate reduces the PV of future payments, which lowers NPV.

#### Cash-Flow Streams

A cash-flow stream is a series of payments received or paid at different times, therefore dependent on its transaction time and amount. Most of the times, the transaction time will occur at regular intervals however, not always. 

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

For a changing instantaneous interest rate, covered in **lesson 1**, using the **yield curve** $\bar r(T)$ also from **lesson 1** :

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

We can also compare the accumulated values at the same future rate instead of comparing present values. 

### Rates of Return

#### Profit and Total Rate of Return 

The profit from an investment is the final value received (with interest) minus the original amount invested. 

Let $P$ be the initial investment and $P_{\mathrm{final}}$ its final value. 

$$
\text{Profit}=P_{\mathrm{final}}-P
$$

The total rate of return, $R$, measures the profit as a proportion of the original investment: 

$$
R=\frac{P_{\mathrm{final}}-P}{P}
$$

#### Annualised Rate of Return 

The ** annualised rate of return ** gives a simple average return per year. 
If an investment lasts $T$ years:

$$
R_{\mathrm{ann}}=\frac{R}{T}
$$

However, this formula does not account for compound growth. A more accurate comparison uses the ••equivalent effective annual interest rate**, $r$: 

$$
P(1+r)^T=P_{\mathrm{final}}
$$

Rearranging this gives: 

$$
r=\left(\frac{P_{\mathrm{final}}}{P}\right)^{1/T}-1
$$

This tells us the yearly compound interest rate needed for an investment to reach its final value. 


#### Internal Rate of Return (IRR)

The **internal rate of return**, known abbreviated as,**IRR**, is used when an investment produces several payments over time. 

It is the interest rate that makes the present value of all future payments equal to the initial investment. 

Let $P$ be the initial investment, $a_i$ is the payment received at time $t_i$, and $r$ is the IRR. 

$$
P=\sum_{i=1}^{n}\frac{a_i}{(1+r)^{t_i}}
$$

We can rearrange this equation to set it equal to zero, which gives:

$$
f(r)=-P+\sum_{i=1}^{n}a_i(1+r)^{-t_i}
$$

The IRR is the value of $r$ that satisfies this equation above: 

$$
f(r)=0
$$

For positive future payments, this equation has a unique solution with $r>-1$.

The **IRR** is extremely useful as it helps people judge whether an investment is worthwhile or not. If its IRR is higher than the available market interest rate, the investment may offer a better rate of return. If the IRR is lower, investing elsewhere may be a better option. 


## My Example: Saving for a New Laptop

### Question

A university student wants to start a small bicycle-repair business. They spend **£3,600 today** on equipment and expect to receive: 

- **£1,200** at the end of Year 1
- **£1,600** at the end of Year 2
- **£1,900** at the end of Year 3

The **effective annual interest rate** is **5.5%**.

Calculate:

1. The **present value** of the future payments (PV)
2. The **Discount factors** and **Net Present Value (NPV)**
3. The **Internal Rate of Return (IRR)**
4. The **Total, Simple Annualised and Effective Annual Return** on an alternative investment.
5. The **Present Value** of a **Perpetuity**
6. The deposit needed today to fund the future payments

Below is a cash-flow timeline to visualise payments being received and being paid out for the question:
      
                   ↑          ↑          ↑
                £1,200     £1,600     £1,900
                   |          |          |
    ---------------|----------|----------|----> Time
         |         |          |          |
        t = 0    t = 1      t = 2       t = 3
         |
         ↓
       £3,600

- **Downward arrow** = Money being paid out
- **Upward arrow** = Money being received
- **t = 0** means the student spends £3,600 today.

### Solution 

**Step 1: Assign the values to a variable**

Let: 
- $P = 3600$ which is the **initial investment**
- $r = 0.055$ which is the **effective annual interest rate**
- $T = 3$ be the length of the investment in years (3 years)
- $a_1 = 1200$, $a_2 = 1600$ and $a_3 = 1900$ be the future payments.

**Step 2: Answer Q1 - Calculate the Present Value (PV)**

Present Value tells us how much future money is worth today

Use the formula: 

$$
PV(a_i)=\frac{a_i}{(1+r)^i}
$$

Here, $a_i$ is the payment received in year $i$. 

**Year 1**

$$
PV_1=\frac{1200}{1.055}
$$

$$
PV_1\approx £1,137.4
$$

**Year 2**

$$
PV_2=\frac{1600}{(1.055)^2}
$$

$$
PV_2\approx £1,437.5
$$

**Year 3**

$$
PV_3=\frac{1900}{(1.055)^3}
$$

$$
PV_3\approx £1,618.1
$$

After calculating for each year, we add the three PV. We use unrounded values:

$$
PV=PV_1+PV_2+PV_3
$$

**Final Answer**:

$$
\boxed{PV\approx £4,193.0}
$$

Therefore, the future payments are worth **£4,193 today**

**Step 3: Answer Q2 - Calculate the Discount Factors and NPV**

A **discount factor (DF)** tells us how much £1 received in the future is worth today. 

Use the formula:

$$
D(t)=\frac{1}{(1+r)^t}
$$

Therefore:

Year 1 (DF) :

$$
D(1)=\frac{1}{1.055}\approx0.9479
$$

Year 2 (DF):

$$
D(2)=\frac{1}{(1.055)^2}\approx0.8985
$$

Year 3 (DF):

$$
D(3)=\frac{1}{(1.055)^3}\approx0.8516
$$

Using the discount factors:

$$
PV=1200D(1)+1600D(2)+1900D(3)
$$

$$
PV\approx £4,193.0
$$

The **Net Present Value (NPV)** is the present value of the future payments - the initial investment. 

$$
NPV=-P+\sum_{i=1}^{3}\frac{a_i}{(1+r)^i}
$$

We then substitute the values given to us from the question:

$$
NPV=-3600+\frac{1200}{1.055}+\frac{1600}{(1.055)^2}+\frac{1900}{(1.055)^3}
$$

I used a round-up function to find an approximate value of the final answer: 

$$
NPV\approx4193.0-3600
$$

**Final answer**

$$
\boxed{NPV\approx £593.0}
$$

As the NPV is > 0 (discussed in the notes above), the investment is financially worth going ahead with at the 5.5% market interest rate.

**Step 4: Solve Q3 - Calculate the Internal Rate of Return (IRR)**

The IRR is the interest rate that makes NPV = 0. 

Use the formula:

$$
0=-P+\sum_{i=1}^{3}\frac{a_i}{(1+r)^i}
$$

We then substitute the values given in the question:

$$
0=-3600+\frac{1200}{1+r}+\frac{1600}{(1+r)^2}+\frac{1900}{(1+r)^3}
$$

We then solve this numerically to get:

$$
\mathrm{IRR}\approx 13.5%\
$$

As 13.5% > 5.5%, the business offers a higher return than the market interest rate.

**Step 5: Solve Q4 - Calculate the Rates of Return**

Now, in theory suppose the student considers another investment which is: buying equipment for **£3,600**, and selling it for **£4,700 after 3 years (t = 3)**, with no other income. 

**(a) Total rate of return**

Use the formula: 

$$
R=\frac{P_{\mathrm{final}}-P}{P}
$$

We then substitute the values given to use from the question: 

$$
R=\frac{4700-3600}{3600}
$$

Final answer: 

$$
\mathrm{IRR}\approx 30.6%\
$$



**(b) Simple annualised rate of return**

We divide the total return by the number of years:

$$
R_{\mathrm{ann}}=\frac{R}{T}
$$

$$
R_{\mathrm{ann}}=\frac{0.305556}{3}
$$

To get a final answer of:

$$
\mathrm{IRR}\approx 10.2%\
$$


**(c) Equivalent effective annual rate**

This is a calculation carried out to show the yearly interest rate needed to grow the investment to its final amount. 

$$
r=\left(\frac{P_{\mathrm{final}}}{P}\right)^{1/T}-1
$$

We then substitute the key values:

$$
r=\left(\frac{4700}{3600}\right)^{1/3}-1
$$

To get a final answer of: 

$$
\boxed{r\approx9.3\%}
$$

The effective annual rate is **9.3%**. 

**Step 6: Solve Q5 - Calculate the present value of a perpetuity** 

Now, suppose another scenario where the student is offered a separate investment paying **£330 every year forever**, starting at the end of Year 1. 

A perpetuity pays the same amount forever - it doesn't change. 

We use the formula:

$$
PV=\frac{a}{r}
$$

We then substitute the key values:

$$
PV=\frac{330}{0.055}
$$

To get a final answer of: 

$$
\boxed{PV=£6,000.0}
$$

Therefore, the perpetuity is worth **£6,000 today**, given the interest rate is at 5.5%. 


**Step 7: Solve Q6 - Calculate the deposit needed to fund future payments**

The student wants to deposit enough money today to find payments of the following: 
- **£1,200, £1,600 and £1,900**
over the next three years.

We use the formula:

$$
PV(\text{deposits})=PV(\text{withdrawals})
$$

Let $X$ be the amount deposited today.

$$
X=\frac{1200}{1.055}+\frac{1600}{(1.055)^2}+\frac{1900}{(1.055)^3}
$$

$$
\boxed{X\approx £4,193.0}
$$

Therefore, the student has to deposit **£4,193 today** to fund (pay-back) the future payments. 

### Conclusion 

The bicycle-repair business has a positive **NPV of £593** and an **IRR of 13.5%**, making it financially worth at the 5.5% market interest rate.

The other calculations shown above are used to value future payments by determining how much money needs to be deposited in today's time. 



