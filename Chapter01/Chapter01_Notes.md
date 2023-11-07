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