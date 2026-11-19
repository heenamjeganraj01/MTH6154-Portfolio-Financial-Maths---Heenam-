# 1. Interest rates

[Back to contents](../README.md)

## Summary

### The Time value of money

Money has a time value because it can earn interest over time. 
An investment made today can grow over time. 
For example, £1,000 invested today can be worth more than £1,000 received next year. 
However, inflation can reduce the purchasing power of money. 
The **principal**,
$P$, 
is the original amount invested or borrowed. 
The **nominal interest rate**,
$r$,
is the stated annual interest rate. 

#### Annual and Compound Interest

Compound interest means earning interest on both your original investment and previously earned interest. 
With annual compounding, interest is added once each year.

After $T$ years:

$P(T) = P(1+r)^T$

For example when T=1: 

$P(1) = P(1+r)$

If interest is compounded $n$ times per year, the balance after $T$ years is: 

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

For semiannual compounding over one year: 

$P(1) = P\left(1+\frac{r}{2}\right)^2$

More frequent compounding, generally increases the accumulated balance if $r$ >0. 

#### Effective Annual Interest Rate

The nominal rate does not fully reflect the effect of compounding. 
The **effective annual rate** measures the actual percentage return earned over one year.
It is calculated as:

$r_{\mathrm{eff}}=\left(1+\frac{r}{n}\right)^n-1$


For interest compounded $n$ times per year: 

$r_{\mathrm{eff}}=\left(1+\frac{r}{n}\right)^n-1$

This allows us to compare investments with different compounding frequencies to be compared fairly.







In your own words, the main ideas of the lesson. Short sentences are fine.

Maths is written between dollar signs. For example `$A = P(1+i)^n$` shows
as $A = P(1+i)^n$, and a displayed formula uses double dollars:

$$
\left(1+\frac{i^{(m)}}{m}\right)^m = 1+i
$$

## My example

A situation you made up (your own numbers, not the ones in the lecture
notes), worked step by step.

## Solved exercises

### Exercise 1.x (from Exercise Sheet 1)

Question, then your solution.

## Spreadsheet

[01-InterestRates.xlsx](../spreadsheets/01-InterestRates.xlsx): what it
does, which cells to change and what to look at.
