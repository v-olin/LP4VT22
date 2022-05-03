# General equations

## Units
$$
Power = Watt [W] \\
Voltage = Volt [V] \\
Current = Ampere [A] \\
Resistance = Ohm [\Omega] \\
Energy = Joule [J] \\
Capacitance = Farad [F] \\

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

## Capacitors and inductors
$$
    q=CV
$$

### Relations
$$
    i = \frac{dq}{dt} = C\frac{dv}{dt} \\
    v = L\frac{di}{dt} \\
    v(t) = \frac{1}{C}\int_{t_0}^ti(t)\ dt + v(t_0)
$$
$$
    v(t)=L\frac{di}{dt} \\
    di=\frac{1}{L}v(t)\ dt\\
    \int_{i_{t_0}}^{i(t)}di=\frac{1}{L}\int_{t_0}^tv(t)\ dt \\
    i(t)=\frac{1}{L}\int_{t_0}^tv(t)\ dt+i(t_0) \\
$$

### Energy stored
$$
    i = C\frac{dv}{dt} \\
    p = iv = Cv\frac{dv}{dt} \\
    w(t) = \int_{t_0}^tp(t)dt \\
    w(t) = \int_{t_0}^tCv\frac{dv}{dt}
    = C \int_{v(t_0)}^{v(t)}vdv = \frac{C}{2} ([v(t)]^2-[v(t_0)]^2)
$$

If $v=0$ at $t_0$:
$$
    w(t)=\frac{Cv^2(t)}{2}\ \ \ \ (q=Cv) \\
    w(t)=\frac{v(t)q(t)}{2}\ \ \ \ C=\frac{q}{v} \\
    w(t)=\frac{q^2(t)}{2C}\ \ \ \ v=\frac{q}{C}
$$

### Capacitors in paralell
*Having three "plates" in parallel is essentially the same as having one large plate (conducting plates)*

$$
    C_{eq} = C_1+C_2+C_3 \\
    i = i_1+i_2+i_3 \\
    i = C\frac{dv}{dt} \\
    i = C_1\frac{dv}{dt} + C_2\frac{dv}{dt} + C_3\frac{dv}{dt} \\
    i = (C_1+C_2+C_3)\frac{dv}{dt}
$$

### Capacitors in series

$$
    C_{eq}=\frac{1}{\frac{1}{C_1}+\frac{1}{C_2}+\frac{1}{C_3}}
$$

### Charging a capacitor
Steady state:
$$
V_C(t)=V_S-V_Se^{\frac{-t}{RC}} \\
V_C(t)=V_S-V_Se^{\frac{-t}{\tau}}
$$

### Inductors
Inductors store energy, since $p(t)=i(t)v(t)=i(L\frac{di}{dt})=\frac{dw}{dt}$
then the energy stored in an inductor is $w=\frac{Li^2}{2}$

### Inductors in series
$$
    L_{eq}=L_1+L_2+ ... + L_n
$$

### Inductors in parallel
$$
    L_{eq}=\frac{1}{\frac{1}{L_1}+\frac{1}{L_2}+...+\frac{1}{L_n}}
$$

### Two-element shortcuts
Two capacitors in series: $C_{eq}=\frac{C_1C_2}{C_1+C_2}$

Two inductors in parallel: $L_{eq}=\frac{L_1L_2}{L_1+L_2}$

Two resistors in parallel: $R_{eq}=\frac{R_1R_2}{R_1+R_2}$

### RC circuits
First-Order RC circuits
$$
    V_c(t)=V_ie^{\frac{-t}{RC}} \\
    \tau=RC \\
    V_c(t)=V_ie^{\frac{-t}{\tau}}
$$

Time constant $\tau=RC$
In one time constant $\tau=RC$ the voltage decays by a factor of $e^{-1}\approx0.368$