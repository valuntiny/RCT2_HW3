Part I. K-stage design
----------------------

### i) What is the goal for Simon’s two-stage design? (10%)

-   minimize the number of patients exposed to a possibly ineffective
    therapy.

-   minimize the sample size under the constraint imposed by the
    operating characteristics of the design

### ii) What is the null and alternative hypothesis for Simon’s two-stage design? (10%)

*H*<sub>0</sub>: the true response rate is less than or equal to some
pre-specified value

*H*<sub>*α*</sub>: the true response rate is greater than some
pre-specified value

### iii) How do you determine the sample size for Simon’s two-stage design? (10%)

Two strategy:

-   optimal design

-   minimax design

### iv) What is the difference between minmax and optimal design for Simon’s two-stage procedure? (10%)

Optimal design aim to minimize the expected number of patients treated
under *H*<sub>0</sub>, while minimax design aim to minimize the total
number of patients enrolled in the study.

### v) What are the drawbacks for Simon’s two-stage design? (10%)

May not allow early termination even if there is a long run of failures
for *p*<sub>0</sub> = 0.10 and above

### vi) How can you overcome the drawbacks? (10%)

Using k-stage designs.

Part II. Write the statistical section of a protocol for a non-superiority trial comparing a testing drug to an placebo control using a continuous outcome.
-----------------------------------------------------------------------------------------------------------------------------------------------------------

We set the hypothesis as *H*<sub>0</sub>:
*p*<sub>*T*</sub> − *p*<sub>*C*</sub> ≥ *Δ*, *H*<sub>1</sub>:
*p*<sub>*T*</sub> − *p*<sub>*C*</sub> &lt; *Δ*. And choose type I error
0.2 and type II error 0.05, and choose superior threshold *Δ* = 0.1,
where we got all them from corresponding superiority trial.

And we will be using one-sided t test, where
$t\_{0} = \\frac{\\hat{p}\_{T} - \\hat{p}\_{C} - \\Delta\_{0}}{\\sigma\\sqrt{1/n\_{T} + 1/n\_{C}}}$.
And
$\\Delta\_{0} = (Z\_{\\alpha} + Z\_{\\beta})\\sigma\\sqrt{\\frac{1}{n\_{T}} - \\frac{1}{n\_{C}}}$.

Given that we could calculate the sample size as
*N* = (*Z*<sub>*α*</sub> + *Z*<sub>*β*</sub>)<sup>2</sup> × \[*p*<sub>*T*</sub>(1 − *p*<sub>*T*</sub>)+*p*<sub>*C*</sub>(1 − *p*<sub>*C*</sub>)\]/*Δ*<sup>2</sup>.
Therefore the necessary number of patients would be 2N.

-   If we reject *H*<sub>0</sub>, we could state that there is
    sufficient evidence to support that treatment is not much better
    than placebo, so we should stop trial.

-   If we fail to reject *H*<sub>0</sub>, we cannot rule out that
    treatment is much better than placebo, so we can move forward to
    next stage.
