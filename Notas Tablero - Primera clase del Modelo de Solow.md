# Dinámica Económica (3009699) — Notas de clase

**Tema:** Crecimiento económico, hechos estilizados y modelo de Solow
**Fuente:** transcripción de los tableros de clase (prof. Camilo Galvis)

> Nota: esta guía transcribe y ordena lo que quedó en el tablero. Donde el tablero tiene una imprecisión, se señala explícitamente.

---

## 1. Punto de partida: el crecimiento de largo plazo

Ejemplo con Colombia, PIB per cápita $y(t)$:

- 1900 $\approx$ US\$1.200
- 2026 $\approx$ US\$10.000

$$\Delta\% y = \frac{10.000 - 1.200}{1.200} = 733{,}3\%$$

Repartido en $n = 126$ años:

$$\frac{733{,}3}{126} = 5{,}82\% \text{ anual}$$

**Precisión importante.** Ese 5,82% es un promedio aritmético simple, no una tasa de crecimiento compuesta. La tasa anual efectiva es:

$$g = \left(\frac{10.000}{1.200}\right)^{1/126} - 1 \approx 1{,}7\% \text{ anual}$$

La diferencia entre ambos cálculos es exactamente el tipo de error que conviene tener claro para el parcial.

---

## 2. Hechos estilizados (Kaldor)

1. El PIB per cápita tiende a crecer en el tiempo.
2. La relación $K/L$ es creciente (la productividad marginal del trabajo crece en el tiempo).
3. La tasa de ganancia del capital como porcentaje del PIB es estable, e incluso ha crecido.

---

## 3. Marx $\leftrightarrow$ Piketty: el debate de fondo

| Marx | Piketty |
|---|---|
| Ley de la tendencia decreciente de la tasa de ganancia | *El capital en el siglo XXI* — visión "propietarista" |
| $\uparrow K/L \Rightarrow$ ejército industrial de reserva $\Rightarrow$ desempleo | Si $r > \Delta\%\text{PIB}$, aumenta $\alpha$ (participación del capital en el PIB) |

**Asignación funcional del ingreso:**

- $K \rightarrow r$ (tasa de ganancia)
- $L \rightarrow w$ (salario)

El esquema de la jornada del tablero ($0 - 4\text{H} - 8\text{H}$) representa el reparto entre trabajo necesario (que se paga como $w$) y plusvalía ($\rho$).

---

## 4. Modelo de Solow — supuestos

> El tablero anota "Solow (1954)"; el artículo original de Robert Solow es de **1956**.

### i) Economía cerrada y sin gobierno

$$Y = C + I \quad \text{(gasto)} \qquad Y = C + S \quad \text{(ingreso)}$$

$$\Longrightarrow \boxed{S = I}$$

### ii) Ahorro tipo keynesiano

$$S(t) = s\,Y(t), \qquad 0 < s < 1 \quad (\text{ejemplo: } s = 0{,}2)$$

$$C(t) = (1-s)\,Y(t)$$

### iii) Capital

$K(t)$ = stock de máquinas, equipos e inmuebles.

Distinción clave: $K$ es un **stock** (patrimonio), $Y$ es un **flujo** (ingreso).

Ejemplo numérico del tablero:

| Variable | Valor |
|---|---|
| $Y_{2026}$ | \$7.000 billones |
| $K_{2026}$ | \$8.000 billones |
| $K_{2025}$ | \$7.800 billones |

**Inversión:**

- Tiempo discreto: $I_t = \Delta K + \delta K$
- Tiempo continuo: $I(t) = \dot{K}(t) + \delta K(t)$

$$\Longrightarrow \dot{K}(t) = I(t) - \delta K(t)$$

donde $\delta$ = tasa de depreciación (ejemplo: 3%).

### iv) Población

$$L(t) = L_0 e^{nt} \qquad \Longrightarrow \qquad \frac{\dot{L}(t)}{L(t)} = n$$

### v) Tecnología (exógena — "otro problema")

$$A(t) = A_0 e^{gt} \qquad \Longrightarrow \qquad \frac{\dot{A}(t)}{A(t)} = g$$

con $A_0$ = tecnología inicial.

### vi) Función de producción

$$Y(t) = f(A, K, L) = A(t)\,K(t)^{\alpha} L(t)^{1-\alpha} \qquad \text{(Cobb-Douglas)}$$

**En términos per cápita**, dividiendo por $L(t)$:

$$\frac{Y(t)}{L(t)} = \frac{A(t) K(t)^{\alpha} L(t)^{1-\alpha}}{L(t)} = A(t)\left(\frac{K(t)}{L(t)}\right)^{\alpha}$$

$$\boxed{y(t) = A(t)\,k(t)^{\alpha}} \qquad \text{con } y = \frac{Y}{L},\; k = \frac{K}{L}$$

**Condiciones de Inada** que debe cumplir la función:

$$\lim_{k \to 0} f'(k) = \infty \qquad \text{(capital escaso} \Rightarrow \text{muy productivo)}$$

$$\lim_{k \to \infty} f'(k) = 0 \qquad \text{(capital abundante} \Rightarrow \text{poco productivo)}$$

Es decir: **rendimientos decrecientes del capital**.

---

## 5. Derivación de la ecuación fundamental

### Paso 1 — Partir de $S = I$

$$s\,Y(t) = \dot{K}(t) + \delta K(t) \qquad \Longrightarrow \qquad \dot{K}(t) = s\,Y(t) - \delta K(t)$$

### Paso 2 — Dividir por $L(t)$

$$\frac{\dot{K}(t)}{L(t)} = s\,\frac{Y(t)}{L(t)} - \delta\,\frac{K(t)}{L(t)} = s\,y(t) - \delta\,k(t) \tag{1}$$

### Paso 3 — El truco: $\dfrac{\dot{K}}{L} \neq \dot{k}$

Hay que derivar bien. Como $k(t) = \dfrac{K(t)}{L(t)}$, entonces $K(t) = k(t)\,L(t)$.

Derivando respecto al tiempo (regla del producto):

$$\frac{\partial K(t)}{\partial t} = k(t)\cdot\frac{\partial L(t)}{\partial t} + L(t)\cdot\frac{\partial k(t)}{\partial t}$$

$$\dot{K}(t) = k(t)\,\dot{L}(t) + L(t)\,\dot{k}(t)$$

Dividiendo todo por $L(t)$:

$$\frac{\dot{K}(t)}{L(t)} = k(t)\,\frac{\dot{L}(t)}{L(t)} + \dot{k}(t) = n\,k(t) + \dot{k}(t)$$

### Paso 4 — Sustituir en (1)

$$n\,k(t) + \dot{k}(t) = s\,y(t) - \delta\,k(t)$$

### Resultado: ecuación fundamental de Solow

$$\boxed{\dot{k}(t) = s\,y(t) - (\delta + n)\,k(t)}$$

---

## 6. Interpretación de cada término

| Término | Significado |
|---|---|
| $\dot{k}(t)$ | Acumulación de capital per cápita |
| $s\,y(t)$ | Ahorro **observado** o efectivo |
| $(\delta + n)\,k(t)$ | Ahorro **requerido** |

El ahorro requerido se descompone en dos partes:

- $\delta k(t)$ → reponer el capital que se deprecia
- $n k(t)$ → dotar de capital a la **nueva población**

**Intuición (los monigotes del tablero):** si hay un trabajador con capital $K$ y llegan más trabajadores, ese mismo $K$ se reparte entre más gente, de modo que $k$ cae. Por eso hay que invertir $nk$ solo para *mantener constante* el capital por persona.

---

## 7. Dinámica y equilibrio de estado estacionario

| Condición | Significado |
|---|---|
| $\dot{k} > 0 \iff s\,y > (\delta+n)k$ | El ahorro efectivo supera al requerido → $k$ crece |
| $\dot{k} = 0 \iff s\,y = (\delta+n)k$ | **Estado estacionario** $k^{*}$ |
| $\dot{k} < 0 \iff s\,y < (\delta+n)k$ | El ahorro no alcanza → $k$ cae |

Por las condiciones de Inada, $s\,y(k)$ es cóncava y $(\delta+n)k$ es una recta que pasa por el origen: se cruzan en un único $k^{*} > 0$, y el sistema converge a ese punto.

**Distinción que hay que mantener clara:** $k^{*}$ es el resultado de *equilibrio de estado estacionario*; el camino desde $k_0$ hasta $k^{*}$ es *dinámica de transición*.

---

## 8. Glosario de notación

| Símbolo | Significado |
|---|---|
| $Y$, $y$ | Producto total / per cápita |
| $K$, $k$ | Capital total / per cápita |
| $L$ | Población o fuerza de trabajo |
| $A$ | Tecnología (productividad total de los factores) |
| $s$ | Propensión marginal a ahorrar |
| $\delta$ | Tasa de depreciación |
| $n$ | Tasa de crecimiento poblacional |
| $g$ | Tasa de crecimiento tecnológico |
| $\alpha$ | Elasticidad del producto al capital / participación del capital |
| $\dot{x}$ | Derivada respecto al tiempo, $dx/dt$ |

---

## Pendiente

El diagrama del estado estacionario (curvas $s\,y(k)$ y $(\delta+n)k$ con el cruce en $k^{*}$) quedó dibujado a medias en el tablero.
