# El tiempo en economía

**Ecuación diferencial:** ecuación que relaciona una función desconocida con una o varias de sus derivadas.

En economía, busca explicar cómo evoluciona un sistema a partir de las reglas que gobiernan su cambio: **ecuación de movimiento**.

---

## Ecuación diferencial lineal de primer orden

$$
\dot{y}(t) + a\,y(t) = u(t) \qquad \Big| \qquad y(t) = y_H + y_P
$$

### El caso homogéneo

$$
\dot{y}(t) + a\,y(t) = 0
$$

$$
\dot{y}(t) = -a\,y(t)
$$

$$
\frac{\dot{y}(t)}{y(t)} = -a
$$

$$
\int \frac{\dot{y}(t)}{y(t)}\,dt = \int -a\,dt
$$

$$
\ln\big(y(t)\big) = -at + c
$$

$$
e^{\ln y} = e^{(-at + c)}
$$

$$
y(t) = e^{-at}\,e^{c}
$$

$$
y(t) = A\,e^{-at}
$$

---

### El caso no homogéneo: particular

$$
\dot{y}(t) + a\,y = b, \quad \text{dado } y \text{ constante}
$$

entonces, $\dot{y}(t) = 0$

$$
a\,y = b
$$

$$
y = \frac{b}{a}
$$

$$
y(t) = \frac{b}{a}
$$

$$
\rightarrow \quad y(t) = y_H + y_P
$$

$$
y(t) = A\,e^{-at} + \frac{b}{a}, \quad \text{dado } a \neq 0
$$

#### Para $t = 0$

$$
y(0) = A\,e^{-a \cdot 0} + \frac{b}{a}
$$

$$
y(0) = A + \frac{b}{a}
$$

$$
\rightarrow \quad A = y(0) - \frac{b}{a}
$$

$$
\boxed{\,y(t) = \left[\,y(0) - \frac{b}{a}\,\right] e^{-at} + \frac{b}{a}\,}
$$
