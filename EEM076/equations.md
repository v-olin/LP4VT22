# General equations

## Units
$$
Power = Watt [W] \\
Voltage = Volt [V] \\
Current = Ampere [A] \\
Resistance = Ohm [\Omega] \\
Energy = Joule [J]
$$

## Ohm's law
$$V = I * R$$

## Conversions
$$
    P = \frac{V^2}{R} = V * I = R * I^2 \\
    V = I * R = \frac{P}{I} = \sqrt{P * R}\\
    I = \sqrt{\frac{P}{R}} = \frac{P}{V} = \frac{V}{R} \\
    R = \frac{V}{I} = \frac{P}{I^2} = \frac{V^2}{P}
$$

## Energy
$$
E = \int_{t_1}^{t_2} p(t) \ dt
$$

## Circuits

### Serial resistance
$$
\begin{equation}
\begin{split} V &= V_1 + V_2 + V_3 \\
    &= i * R_1 + i * R_2 + i * R_3 \\
    &= i * (R_1 + R_2 + R_3)    
\end{split}
\end{equation}
$$

### Parallel resistance
$$
\begin{equation}
\begin{split} i &= i_1 + i_2 + i_3 \\
    &= v/R_1 + v/R_2 + v/R_3 \\
    &= v * (R_1^{-1} + R_2^{-1} + R_3^{-1})
\end{split}
\end{equation}
$$

## Voltage and Current
### Voltage divider
$$
R_{eq} = R_1 + R_2 + R_3,
i = V_{total} / R_{eq} \\
V_1 = i * R_1 = V_{total} * R_1/(R_1+R_2+R_3) \\
V_2 = i * R_2 = V_{total} * R_2/(R_1+R_2+R_3) \\
V_3 = i * R_3 = V_{total} * R_3/(R_1+R_2+R_3)
$$

### Current divider
**TODO**