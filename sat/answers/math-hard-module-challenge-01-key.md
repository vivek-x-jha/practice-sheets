# SAT Math: Hard-Module Challenge 1 — Answer Key

Original, unofficial practice. Suggested time: 30 minutes for 12 questions. Difficulty is a design target, not an official College Board calibration; this set does not predict an SAT score.

| Question | Answer | Value |
| --- | --- | --- |
| 1 | A | -4 |
| 2 | C | 52 |
| 3 | B | 19 |
| 4 | D | 11/31 |
| 5 | C | 3 |
| 6 | D | 18 |
| 7 | C | 5,256 |
| 8 | B | 1,216 |
| 9 | B | -26/5 |
| 10 | A | 26 + 10√13 |
| 11 | C | 9 |
| 12 | A | 23 |

## Explanations

1. **A — -4.** For the system not to have a unique solution, its coefficient determinant must be zero: `(a-2)(a+1)-18=0`, or `(a-5)(a+4)=0`. At `a=5`, the second equation is twice the first, so there are infinitely many solutions. At `a=-4`, the equations are `-6x+3y=7` and `6x-3y=14`; adding them gives `0=21`. Only `a=-4` gives no solution.

2. **C — 52.** Since `f(2)=f(8)`, the axis of symmetry is `x=5`. Write `f(x)=a(x-5)^2+d`. The given values imply `9a+d=24` and `a+d=-8`, so `a=4` and `d=-12`. The requested sum is `f(1)=4(1-5)^2-12=52`, not the constant term `f(0)=88`.

3. **B — 19.** Over the equal input intervals, the output differences are `35-11=24` and `131-35=96`. Their ratio is `b^2=96/24=4`, so `b=2`. Now `a+c=11` and `4a+c=35` give `a=8` and `c=3`. Thus `g(1)=8(2)+3=19`. Ratios of the original outputs do not give the growth factor because of the added constant.

4. **D — 11/31.** Let `p` be the fraction of all components made by B. Then `0.04(1-p)+0.12p=0.07`, giving `p=3/8`. The fraction of all components that are both from B and nondefective is `(3/8)(0.88)=33/100`. Since `93/100` of all components are nondefective, the requested conditional probability is `(33/100)/(93/100)=11/31`. The denominator is the nondefective group, not the entire day's production.

5. **C — 3.** The original expression requires `x != 3`. Factoring reduces the equation to `x+3=kx`. At `k=1`, this gives `3=0`, so there is no solution. For `k != 1`, the candidate solution is `x=3/(k-1)`. That candidate is excluded when `k=2`, because it equals 3. All other values of `k` give one valid solution. The requested sum is `1+2=3`.

6. **D — 18.** At `k=3`, the equation is linear: `12x+3=0`, which has one solution. For `k != 3`, it is quadratic and has exactly one real solution when `12^2-4(k-3)(3)=0`. This gives `k=15`. Both values qualify, so their sum is `3+15=18`. The equation was not stated to remain quadratic for every `k`.

7. **C — 5,256.** Let `n` be the number of $3 price increases. Ticket price is `30+3n`, and predicted sales are `240-12n`. After the $6 per-ticket expense and the fixed expense, profit is `(24+3n)(240-12n)-1800 = -36n^2+432n+3960 = 5256-36(n-6)^2`. Its maximum is $5,256 at `n=6`: a $48 price and 168 tickets. Maximizing revenue alone would instead give a $45 price and a smaller profit of $5,220.

8. **B — 1,216.** The surface-area ratio `9:25` gives a length ratio `3:5` and a volume ratio `27:125`. Write the volumes as `27u` and `125u`. Then `98u=784`, so `u=8`. Their sum is `152u=1216` cubic centimeters. The surface-area ratio cannot be applied directly to volume.

9. **B — -26/5.** Substitute `y=2x+1` into the circle equation to obtain `5x^2+6x+(7+c)=0`. Tangency means exactly one intersection, so the discriminant is zero: `36-20(7+c)=0`. Thus `c=-26/5`. As a check, the circle has center `(5,-3)` and radius squared `34-c=196/5`, which is positive.

10. **A — 26 + 10√13.** Set `AD=4t` and `DB=9t`, with `t>0`. The similar right triangles give `CD^2=AD·DB=36t^2`, so `CD=6t` and `AB=13t`. The area condition is `(1/2)(13t)(6t)=156`, giving `t=2`. The legs are `AC=sqrt(AD·AB)=4sqrt(13)` and `BC=sqrt(DB·AB)=6sqrt(13)`, while `AB=26`. Their sum is `26+10sqrt(13)`.

11. **C — 9.** Complete the square: `x^2-8x+7=(x-4)^2-9`. For `k>0`, the equation separates into `(x-4)^2=9+k` and `(x-4)^2=9-k`. The first always has two solutions. The second has two solutions for `0<k<9`, one for `k=9`, and none for `k>9`. Since the two branches cannot share a solution when `k>0`, exactly three distinct solutions occur only at `k=9`.

12. **A — 23.** Square the given equation: `2^(2x)+2(2^x)(2^(-x))+2^(-2x)=25`. The product in the middle is 1, so the requested value is `25-2=23`. Omitting the cross term would incorrectly give 25.

## Design references

The content scope and concise, four-option presentation were informed by College Board's *Digital SAT Sample Questions and Answer Explanations*, *Student Question Bank: Math Questions*, and *The Math Section: Overview*. The questions and explanations here are original, not reproduced official items. The set deliberately concentrates on challenging reasoning rather than matching a full module's topic proportions or difficulty distribution.
