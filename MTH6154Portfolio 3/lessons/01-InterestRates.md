# 1. Interest rates

[Back to contents](../README.md)

## Summary

#### The Time value of money

Money has a different value depending on when we receive it.
For example, £5,000 received today can be worth more than £15,000 received next year because we can put it in a bank and earn interest.
This means an investment made today can grow over time. 
However, inflation can also make the same £1,000 worth less in terms of what it can buy.

The starting amount we invest or borrow is called the **principal**,
$P$. 

#### Nominal Annual Interest Rate

The **nominal annual interest rate**,
$r$,
is the stated annual interest rate expressed as a decimal. 
For example, 5%, is written as $r$ = 0.05. 

If we borrow $P$ for one year, the interest charged is $rP$. The total amount we owe is therefore: 
$P$ + $rP$ = $P(1+r)$. 
The same applies to a savings situation.

#### Compound Interest

Compound interest means earning interest on both your original money and previously earned interest. This means the balance can grow faster over time.

When interest is added once a year, called **annual compounding**, the amount after $T$ years is:
$P(T)$ = $P(1+r)^T$

For example when T=1: 

$P(1) = P(1+r)$

However, banks may add interest more frequently. If interest is compounded $n$ times per year for $T$ years, where each period uses the rate $r/n$: 

$P(T) = P\left(1+\frac{r}{n}\right)^{nT}$

where: 
- $P$ = initial principal
- $P(T)$ = accumulated balance
- $r$ = nominal annual interest rate
- $n$ = compounding periods per year
- $T$ = investment duration in years

Examples of compounding frequencies: 

- Annually: $n=1$
- Semiannually: $n=2$
- Quarterly: $n=4$
- Monthly: $n=12$
- Daily: $n=365$

Here, T is the number of years. 

For semiannual compounding (n=2):
$P(T) = P\left(1+\frac{r}{2}\right)^{2T}$

More frequent compounding, generally increases the accumulated balance if $r$ >0. 

#### Effective Annual Interest Rate

The **effective annual rate**, **$r_{\mathrm{eff}}$**, measures the actual yearly return, after accounting for how often interest is added:

$r_{\mathrm{eff}}=\left(1+\frac{r}{n}\right)^n-1$

This allows rates with different compounding frequencies to be compared.

#### Continuous Compounding 
With **continuous compounding**, interest is added increasingly frequently. In notation: $n\to\infty\$: 

$\lim_{n\to\infty}P\left(1+\frac rn\right)^{nT}
=Pe^{rT}$

Therefore: 

$P(T)=Pe^{rT},\qquad r_{\mathrm{eff}}=e^r-1$
Using the **effective annual rate**, we can also write $\(P(T)=P(1+r_{\mathrm{eff}})^T\)$. These formulas also apply to loans when no repayments are made. 

#### Doubling Time

**Doubling Time** tells us how long money takes to double under **continuous compounding**:

Let $T$ represent the amount of years it takes an amount $P$ to double, we have 

$\[2P=Pe^{rT}\quad\Rightarrow\quad\boxed{T=\frac{\ln2}{r}\approx\frac{0.693}{r}}\]$, by rearranging to solve $T$.

The **Rule of 72** is a quick estimate: 
$\[T\approx\frac{72}{R}\]$,
where $R$ is the interest rate written as a percentage.

### Variable Interest Rates
#### Instantaneous Interest Rate
Interest rates can change over time. The **instantaneous interest rate $r(t)$** tells us the rate at a particular moment. 

Let **$r(t)$** be the interest rate at time **$t$**, **$P(t)$** the balance at that time, and **$P(0)$** the starting balance at **time zero**. 

Over a very short time interval $h$, the interest rate is approximately constant. Using $\(e^{r(t)h}\approx1+r(t)h\)$ we can calculate the amount of interest that occurs between time $t$ and $t+h$: 

$\[P(t+h)\approx P(t)e^{r(t)h}\approx P(t)(1+r(t)h)\]$
This means that the balance is approximately the current balance plus the interest earned. As $h$ approaches zero:

$\[\{P'(t)=P(t)r(t)}\]$

Here, $P'(t)$, means how quickly the balance changes over time. 
To find the balance, we need to divide both sides of $\[\{P'(t)=P(t)r(t)}\]$
by $P(t)$ and **integrate** from time $0$ to time $t$ to calculate the total growth.

$\frac{P'(t)}{P(t)}=r(t)\quad\Rightarrow\quad\ln P(t)-\ln P(0)=\int_0^t r(u)\ du$

The symbol $\int$ means integration, and $u$ represents time within the interval. We subtract $\ln P(0)$ because we are measuring growth from the **initial balance** to the balance at time $t$.

Removing the logarithm using the exponential function $e^x$ gives:

$P(t)=P(0)e^{\int_0^t r(u)\ du}$

This formula calculates the future balance when interest rate is not constant. If the rate stays constant, $r(t) = r$, it simplifies to: 

$P(t)=P(0)e^{rt}$

#### Yield Curve 

The **yield curve**, written as $\bar r(t)$, gives the average **instantaneous rate** from time $0$ to time $t$: 

$\bar r(t)=\frac{1}{t}\int_0^t r(u)\ du$

Using this average rate, the balance becomes: 

$P(t)=P(0)e^{t\bar r(t)}$

The effective **annual interest rate** for an investment lasting $T$ years is: 

$r_{\mathrm{eff}}(T)=e^{\bar r(T)}-1$

### Inflation 

**Inflation** means prices increase over time, which reduces the purchasing power of money. 

Let $r_{\mathrm{inf}}$ be the annual inflation rate, and  $r_a$ the ** real interest rate**, which measures how much our purchasing power increases. 

If the effective annual interest rate is $r$, the balance after one year is $P(1+r)$, but its purchasing power in today's money is: 

$\frac{P(1+r)}{1+r_{\mathrm{inf}}}$

Therefore, the real interest rate is: 

$r_a=\frac{1+r}{1+r_{\mathrm{inf}}}-1=\frac{r-r_{\mathrm{inf}}}{1+r_{\mathrm{inf}}}$

If interest is compounded more than once a year, use the effective annual rate $r_{\mathrm{eff}}$ instead:

$r_a=\frac{r_{\mathrm{eff}}-r_{\mathrm{inf}}}{1+r_{\mathrm{inf}}}$

When inflation is small, we can approximate it by:

$r_a\approx r_{\mathrm{eff}}-r_{\mathrm{inf}}$

This shows that earning interest does not always mean gaining purchasing power, because inflation can reduce the real value of our savings over time.



## My Example: Saving for a New Laptop

### Question

A university student wants to save money to buy a new laptop in the future. They deposit **£1,850** into a savings account offering a **nominal annual interest rate of 4.8%, compounded monthly**. The student leaves the money untouched for **3 years**.

Calculate:

1. The total balance after 3 years.
2. The total interest earned.
3. The effective annual interest rate.

### Solution

**Step 1: Identify the values**

Let:

- $P=£1,850$ be the initial deposit (principal).
- $r=0.048$ be the nominal annual interest rate.
- $n=12$ be the number of compounding periods per year.
- $T=3$ be the investment duration in years.

**Step 2: Calculate the balance after 3 years**

Since interest is compounded monthly, we use the compound interest formula:

**$P(T)=P\left(1+\frac{r}{n}\right)^{nT}$**

Substituting the values we get:

**$P(3)=1850\left(1+\frac{0.048}{12}\right)^{12\times3}$**

$=1850(1.004)^{36}$

$\boxed{P(3)=£2,135.92}$

Therefore, the student will have **£2,135.92** after 3 years.

**Step 3: Calculate the total interest earned**

The total interest is the final balance minus the original deposit:

$\text{Interest}=P(3)-P$

$=2135.92-1850$

$\boxed{\text{Interest}=£285.92}$

**Step 4: Calculate the effective annual interest rate**

The **effective annual rate** accounts for how often interest is added throughout the year:

$r_{\mathrm{eff}}=\left(1+\frac{r}{n}\right)^n-1$

Substituting the values:

$r_{\mathrm{eff}}=\left(1+\frac{0.048}{12}\right)^{12}-1$

$=(1.004)^{12}-1$

$\approx0.0490702$

$r_{\mathrm{eff}} \approx 4.91\%}$

### Conclusion

After 3 years, the student's original deposit of **£1,850 grows to £2,135.92**, earning **£285.92 in interest**. Although the **nominal annual interest rate is 4.8%**, monthly compounding increases the effective annual rate to approximately **4.91%**.

This shows how compound interest helps savings grow over time, as interest is earned on both the original deposit and previously accumulated interest.


## Solved Exercises

### Exercise 1

Suppose you put £700 in a bank account with nominal interest rate 3%.

**(a) How much money will be in the bank account three years from now if the interest is:**

**(i) Compounded annually?**

For annual compounding, we use:

$P(T)=P(1+r)^T$

Substituting $P=700$, $r=0.03$ and $T=3$:

$
\begin{aligned}
P(3)&=700(1+0.03)^3\\
&=700(1.03)^3\\
&=764.91\\
&\approx765
\end{aligned}
$

Therefore, the balance is approximately **£765**.

**(ii) Compounded monthly?**

Interest is added 12 times per year, so $n=12$.

Using the compound interest formula:

$$
P(T)=P\left(1+\frac{r}{n}\right)^{nT}
$$

Substituting the values:

$$
\begin{aligned}
P(3)&=700\left(1+\frac{0.03}{12}\right)^{12\times3}\\
&=700(1.0025)^{36}\\
&\approx765.84\\
&\approx766
\end{aligned}
$$

Therefore, the balance is approximately **£766**.

**(iii) Compounded semi-annually?**

Interest is added twice per year, so $n=2$.

$$
P(T)=P\left(1+\frac{r}{2}\right)^{2T}
$$

Substituting the values:

$$
\begin{aligned}
P(3)&=700\left(1+\frac{0.03}{2}\right)^{2\times3}\\
&=700(1.015)^6\\
&\approx765.41\\
&\approx765
\end{aligned}
$$

Therefore, the balance is approximately **£765**.

**(iv) Compounded continuously?**

For continuous compounding, we use:

$$
P(T)=Pe^{rT}
$$

Substituting the values:

$$
\begin{aligned}
P(3)&=700e^{0.03\times3}\\
&=700e^{0.09}\\
&\approx765.92\\
&\approx766
\end{aligned}
$$

Therefore, the balance is approximately **£766**.

**(b) Find the effective interest rates $r_{\mathrm{eff}}$ for each case (i)–(iv) from part (a).**

For periodic compounding, we use:

$$
r_{\mathrm{eff}}=\left(1+\frac{r}{n}\right)^n-1
$$

**(i) Compounded annually**

Since $n=1$:

$$
\begin{aligned}
r_{\mathrm{eff}}&=(1+0.03)^1-1\\
&=1.03-1\\
&=0.03\\
&=3.00\%
\end{aligned}
$$

**(ii) Compounded monthly**

Since $n=12$:

$$
\begin{aligned}
r_{\mathrm{eff}}&=\left(1+\frac{0.03}{12}\right)^{12}-1\\
&=(1.0025)^{12}-1\\
&\approx0.030416\\
&\approx3.04\%
\end{aligned}
$$

**(iii) Compounded semi-annually**

Since $n=2$:

$$
\begin{aligned}
r_{\mathrm{eff}}&=\left(1+\frac{0.03}{2}\right)^2-1\\
&=(1.015)^2-1\\
&=0.030225\\
&\approx3.02\%
\end{aligned}
$$

**(iv) Compounded continuously**

For continuous compounding, we use:

$$
r_{\mathrm{eff}}=e^r-1
$$

Substituting $r=0.03$:

$$
\begin{aligned}
r_{\mathrm{eff}}&=e^{0.03}-1\\
&\approx0.030455\\
&\approx3.05\%
\end{aligned}
$$

**(c) Suppose the inflation rate is $r_{\mathrm{inf}}=2\%$. Calculate the 'inflation adjusted interest rate' for each case (i)–(iv) from part (a).**

The inflation-adjusted interest rate is calculated using:

$$
r_a=\frac{r_{\mathrm{eff}}-r_{\mathrm{inf}}}{1+r_{\mathrm{inf}}}
$$

Since inflation is 2%, $r_{\mathrm{inf}}=0.02$.

Using the rounded effective rates from part (b), as in the lecturer's solutions:

**(i) Compounded annually**

$$
\begin{aligned}
r_a&=\frac{0.0300-0.02}{1+0.02}\\
&=\frac{0.01}{1.02}\\
&\approx0.009804\\
&\approx0.98\%
\end{aligned}
$$

**(ii) Compounded monthly**

$$
\begin{aligned}
r_a&=\frac{0.0304-0.02}{1+0.02}\\
&=\frac{0.0104}{1.02}\\
&\approx0.010196\\
&\approx1.02\%
\end{aligned}
$$

**(iii) Compounded semi-annually**

$$
\begin{aligned}
r_a&=\frac{0.0302-0.02}{1+0.02}\\
&=\frac{0.0102}{1.02}\\
&=0.01\\
&=1.00\%
\end{aligned}
$$

**(iv) Compounded continuously**

$$
\begin{aligned}
r_a&=\frac{0.0305-0.02}{1+0.02}\\
&=\frac{0.0105}{1.02}\\
&\approx0.010294\\
&\approx1.03\%
\end{aligned}
$$

**(d) Suppose interest is compounded semi-annually. How long will it take for the bank balance to grow to £1,000?**

Let $T$ be the time in years.

For semi-annual compounding:

$$
P(T)=P\left(1+\frac{r}{2}\right)^{2T}
$$

**Step 1: Substitute the values**

$$
1000=700\left(1+\frac{0.03}{2}\right)^{2T}
$$

Simplifying:

$$
1000=700(1.015)^{2T}
$$

**Step 2: Take natural logarithms**

$$
\ln(1000)=\ln(700)+2T\ln(1.015)
$$

**Step 3: Rearrange to find $T$**

$$
\begin{aligned}
T&=\frac{\ln(1000)-\ln(700)}{2\ln(1.015)}\\
&\approx11.98\\
&\approx12.0\text{ years}
\end{aligned}
$$

Therefore, it takes approximately **12 years** for the balance to reach £1,000.

---

### Exercise 3

Suppose $P$ is deposited in a bank account with interest continuously compounded at rate $r(t)$. Write down an expression, in terms of $r(t)$, for:

**(a) The yield curve $\bar r(t)$.**

The yield curve represents the average instantaneous interest rate over the period from $0$ to $t$.

**Step 1: Integrate the interest rate**

$$
\int_0^t r(s)\,ds
$$

**Step 2: Divide by the time interval**

Dividing by $t$ gives the average interest rate:

$$
\bar r(t)=\frac{1}{t}\int_0^t r(s)\,ds
$$

Therefore, the yield curve is:

$$
\bar r(t)=\frac{1}{t}\int_0^t r(s)\,ds
$$

**(b) The bank balance at time $t$.**

For continuous compounding with a variable interest rate:

$$
P'(t)=P(t)r(t)
$$

**Step 1: Divide both sides by $P(t)$**

$$
\frac{P'(t)}{P(t)}=r(t)
$$

**Step 2: Integrate both sides from $0$ to $t$**

$$
\ln P(t)-\ln P(0)=\int_0^t r(s)\,ds
$$

**Step 3: Rearrange using the exponential function**

Since $P(0)=P$:

$$
P(t)=P\exp\left(\int_0^t r(s)\,ds\right)
$$

**Step 4: Substitute the yield curve**

From part (a):

$$
t\bar r(t)=\int_0^t r(s)\,ds
$$

Therefore:

$$
P(t)=Pe^{t\bar r(t)}
=P\exp\left(\int_0^t r(s)\,ds\right)
$$




## Spreadsheet

[01-InterestRates.xlsx](../spreadsheets/01-InterestRates.xlsx): what it
does, which cells to change and what to look at.
