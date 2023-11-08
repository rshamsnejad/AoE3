---
title: "The Art Of Electronics 3rd Edition - Notes on Chapter 01"
date: 2023-11-07
geometry: margin=2cm
output: pdf_document
---

# The Art Of Electronics 3rd edition
*Notes on Chapter 01*

* Thevenin trick to get output/input impedance
* Capacitor = frequency dependant resistor (disregarding phase shift!)

## 1.7 Impedance and Reactance
### 1.7.1 Frequency analysis of reactive circuits

#### A. RC lowpass filter (approximate)
\ 

![RC passive lowpass filter](figure_1.90.png){#fig:rclowpass width=50%}

$$
\frac{V_{out}}{V_{in}} \approx \frac{X_C}{R + X_C} = \frac{1}{1 + \omega R C}
$$

#### B. RC highpass filter (approximate)
\ 

![RC passive highpass filter](figure_1.92.png){#fig:rchighpass width=50%}

$$
\frac{V_{out}}{V_{in}} \approx \frac{R}{R + X_C} = \frac{\omega R C}{1 + \omega R C}
$$

#### C. Blocking capacitor
\ 

![Blocking capacitor](figure_1.93.png){#fig:rcblocking width=50%}

For a pulse of duration T to not be distorted while going through the blocking
capacitor:

Choose R to fit the pre-amp's output resistance and amplifier's input
resistance, then choose C so that $RC \gg T$

#### D. Driving and loading RC filters
\ 

![Cascading RC filters](exercise_1.24.png){#fig:rccascade width=100%}

For this configuration with a desired highpass filter of cutoff frequency $f_1$
and lowpass of cutoff frequency $f_2$:

1. Determine $R_{source}$
1. Set $R_1 \ge 10 \cdot R_{source}$
1. Set $R_2 \ge 10 \cdot R_1$
1. It gives $R_{load} \ge 10 \cdot R_2$
1. Calculate $C_1 = \frac{1}{2\pi \cdot f_1 \cdot R_1}$
1. Calculate $C_2 = \frac{1}{2\pi \cdot f_2 \cdot R_2}$
1. Adjust $C_1$ and $C_2$ empirically if the accuracy is not already good enough

##### Examples
\ 

![Cascading RC filters with $100 \Omega$ source](exercise_1.24-100R-source.png){#fig:rccascade-100 width=100%}

![Cascading RC filters with $5 \Omega$ source](exercise_1.24-5R-source.png){#fig:rccascade-5 width=100%}