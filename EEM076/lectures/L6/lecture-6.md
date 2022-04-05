# Lecture 6

## Work
To move charges apart from one another, they must do work.
![work](work.png)
$$
    W=F\overrightharpoon{r} \\
    \overrightharpoon{F}_{12}=k_e\frac{q_1q_2}{r^2}\hat{r}_{12} \\
    W=\int_R^{\infty}\overrightharpoon{F}\cdot d\overrightharpoon{r} = -k_eq_1q_2
    \int_R^{\infty}\frac{d\overrightharpoon{r}}{r^2}=\frac{k_eq_1q_2}{R}
$$

### Work in an electric field
Now consider a charge moving in the direction of a uniform electric field.
![el](elwork.png)
$$
    W=\overrightharpoon{F}\cdot d\overrightharpoon{r} \\
    \overrightharpoon{F}_E=q\overrightharpoon{E} \\
    W=-\int_A^B\overrightharpoon{F}\cdot d\overrightharpoon{r}=-\int_A^Bq\overrightharpoon{E}
    \cdot d\overrightharpoon{r}=-qE_0\int_A^Bd\overrightharpoon{r}=-qE_0d
$$

If moving perpendicular to a uniform electric field, what is the work?
Answer: 0, cause $\int_A^Bd\overrightharpoon{r}=0$

### Potential Energy
Another way to write work is as the difference in potential energy.
$$
W=\Delta U=-\int_A^B\overrightharpoon{F}\cdot d\overrightharpoon{r}
$$

This potential is proportional ot the charge $\overrightharpoon{F}_E=q\overrightharpoon{E}$

### Electric potential
Normalizing this by the charge gives us:
$$
    \frac{W}{q}=-\int_A^B\overrightharpoon{E}\cdot d\overrightharpoon{r}=\Delta V
$$

Recall the definition of voltage from L1: $[\Delta V]=\frac{J}{C}$

### Voltage
What happens if we calculate the work across a closed path?
$$
    -\oint\overrightharpoon{F}\cdot d\overrightharpoon{r}=0
$$

![matrix](matr.png)

## Electric field and voltage

### Equipotential curves
We can work backwards from a known voltage to calculate the electric field.
![equipo](equ.png)
$$
    \Delta V = -\int_A^B\overrightharpoon{E}\cdot d\overrightharpoon{r} \\
    dV=-\overrightharpoon{E}\cdot d\overrightharpoon{r} \\
    \overrightharpoon{E}=-\frac{dV}{d\overrightharpoon{r}}=-\nabla V
$$

Equipotential curves show regions of constant potential.
The electric field $\overrightharpoon{E}$ is perpendicular (normal) to these curves.
![equ2](equ2.png)
(Yellow: EF lines, Blue: EPC lines)

## Capacitance
Capacitance is the ability for an electric potential to hold a charge.
$$
    C=\frac{Q}{|\Delta V|}
$$

### Capacitors
Two isolated plates with equal and opposite charges: $\plusmn Q$
When charged, creates a voltage difference across the plates.
What is the voltage?

![plates](cond.png)

Assume:
Surface area $A$
Surface charge density $\sigma$
$
    Q=\sigma A \\
$

![pillbox](pillbox.png)
$$
    \Phi=\oiint\overrightharpoon{E}\cdot d\overrightharpoon{A}=\frac{q_{enc}}{\varepsilon_0} \\
    EA_1=\frac{Q}{\varepsilon_0}=\frac{\sigma A_1}{\varepsilon_0} \\
    E=\frac{\sigma}{\varepsilon_0}=\frac{Q}{\varepsilon_0A}
$$

![2dplates](2d.png)
$$
    \Delta V=-\int_+^-\overrightharpoon{E}\cdot d\overrightharpoon{r}=-Ed \\
    Ed=\frac{Q}{\varepsilon_0A}d \\
    C=\frac{Q}{|\Delta V|}=\frac{Q}{\frac{Q}{\varepsilon_0A}d}=\varepsilon_0\frac{A}{d}
$$

### Stored energy in a capacitor
![man](man.png)
Recall:
$$
    \frac{W}{q}=-\int_A^B\overrightharpoon{E}\cdot d\overrightharpoon{s}=\Delta V \\
    dW = dq\Delta V=dq\frac{q}{C} \\
    W = \int dW=\frac{1}{C}\int_0^Qq\ dq=\frac{1}{C}\frac{Q^2}{2}
$$

How is the potential energy stored?
$$
    U=\frac{1}{C}\frac{Q^2}{2}=\frac{1}{2}Q|\Delta V|=\frac{1}{2}C|\Delta V|^2 \\
    \frac{1}{2}C|\Delta V|^2 =\frac{1}{2}\frac{\varepsilon_0A}{d}(Ed)^2=
    \frac{1}{2}\varepsilon_0E^2(Ad)=u x (volume) \\
    u = (E\ field\ density)=\frac{\varepsilon_0E^2}{2}
$$