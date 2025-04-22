# Produto Escalar e Multiplicação de Matrizes


## Produto Escalar

O **produto escalar** ou **produto interno** dos vetores de dimensão $\color{red}{n}$ $\mathbf{\color{red}{a}}$ e $\mathbf{\color{red}{b}}$ é a soma dos produtos dos elementos correspondetes. Dessa maneira, se $\mathbf{\color{red}{a}} = \begin{bmatrix} a_1 \\ a_2 \\ \vdots \\ a_n \end{bmatrix}$, $\; \mathbf{\color{red}{b}} = \begin{bmatrix} b_1 \\ b_2 \\ \vdots \\ b_n \end{bmatrix}$, então:

```{math}
:label: eq06
    \mathbf{a} \cdot \mathbf{b} = a_1 b_1 + a_2 b_2 + \cdots + a_n b_n = \sum_{i=1}^{n} a_i b_i.
```

:::{include} examples.md
:start-after: <!-- Start Exemple 1.12 -->
:end-before: <!-- End Exemple 1.12 -->
:::

:::{include} examples.md
:start-after: <!-- Start Exemple 1.13 -->
:end-before: <!-- End Exemple 1.13 -->
:::

## Multiplicação de Matrizes

Se $\color{red}{A = [a_{ij}]}$ é uma matriz $\color{red}{m \times p}$ e $\color{red}{B = [b_{ij}]}$ é uma matriz $\color{red}{p \times n}$, então o **produto** de $\color{red}{A}$ e $\color{red}{B}$, representado por $\color{red}{AB}$, é a matriz $\color{red}{m \times n}$, $\color{red}{C = [c_{ij}]}$ , definida por:

```{math}
:label: eq07
    c_{ij} = a_{i1}b_{1j} + a_{i2}b_{2j} + \cdots + a_{ip}b_{pj} = \sum_{k=1}^{p} a_{ik}b_{kj}, \quad (1 \leq i \leq m,\; 1 \leq j \leq n)
```

:::{include} examples.md
:start-after: <!-- Start Exemple 1.14 -->
:end-before: <!-- End Exemple 1.14 -->
:::

:::{include} examples.md
:start-after: <!-- Start Exemple 1.15 -->
:end-before: <!-- End Exemple 1.15 -->
:::



```{admonition} Atenção!
:class: warning
Observe que o produto de $\color{red}{A}$ e $\color{red}{B}$ é definido apenas quando o número de colunas de $\color{red}{A}$ é exatamente igual ao número de linhas de $\color{red}{B}$.
```

## Sistemas Lineares

Considere o sistema linear de $\color{red}m$ equações em $\color{red}{n}$ incógnitas:

```{math}
:label: eq08
    \begin{matrix}
        a_{11}x_{1} & + & a_{12}x_{2} & + & \cdots & + & a_{1n}x_{n} & = & b_{1}    \\
        a_{21}x_{1} & + & a_{22}x_{2} & + & \cdots & + & a_{2n}x_{n} & = & b_{2}    \\
        \vdots      &   & \vdots      &   &        &   & \vdots      &   & \vdots   \\
        a_{m1}x_{1} & + & a_{m2}x_{2} & + & \cdots & + & a_{mn}x_{n} & = & b_{m}    \\
    \end{matrix}
```

Definimos agora as seguintes matrizes:

$$
    A = \begin{bmatrix}
        a_{11} & a_{12} & \cdots & a_{1n} \\
        a_{21} & a_{22} & \cdots & a_{2n} \\
        \vdots & \vdots & \ddots & \vdots \\
        a_{m1} & a_{m2} & \cdots & a_{mn}
    \end{bmatrix},
        \quad
    x = \begin{bmatrix}
        x_1 \\
        x_2 \\
        \vdots \\
        x_n
    \end{bmatrix},
        \quad
    b = \begin{bmatrix}
        b_1 \\
        b_2 \\
        \vdots \\
        b_m
    \end{bmatrix}
$$

Então

$$
    Ax = \begin{bmatrix}
        a_{11} & a_{12} & \cdots & a_{1n} \\
        a_{21} & a_{22} & \cdots & a_{2n} \\
        \vdots & \vdots & \ddots & \vdots \\
        a_{m1} & a_{m2} & \cdots & a_{mn}
    \end{bmatrix}
    \begin{bmatrix}
        x_1 \\
        x_2 \\
        \vdots \\
        x_n
    \end{bmatrix}
        =
    \begin{bmatrix}
        a_{11}x_1 + a_{12}x_2 + \cdots + a_{1n}x_n \\
        a_{21}x_1 + a_{22}x_2 + \cdots + a_{2n}x_n \\
        \vdots \\
        a_{m1}x_1 + a_{m2}x_2 + \cdots + a_{mn}x_n
    \end{bmatrix}
$$

Os elementos no produto $\color{red}{Ax}$ são simplesmente as expressões à esquerda dos sinais de igualdade em {math:numref}`eq08`. Por esse motivo, o sistema linear {math:numref}`eq08` pode ser escrito na forma de matriz da seguinte maneira:

$$
Ax = b.
$$

A matriz $\color{red}{A}$ é chamada **matriz de coeficientes** do sistema linear {math:numref}`eq08` e a matriz

$$
    \left[
        \begin{array}{cccc|c}
            a_{11} & a_{12} & \cdots & a_{1n} & b_1 \\
            a_{21} & a_{22} & \cdots & a_{2n} & b_2 \\
            \vdots & \vdots & \ddots & \vdots & \vdots \\
            a_{m1} & a_{m2} & \cdots & a_{mn} & b_m
        \end{array}
    \right],
$$

obtida juntando-se a coluna $\color{red}{b}$ a $\color{red}{A}$, é chamada **matriz aumentada** do sistema linear {math:numref}`eq08`. A matriz aumentada de {math:numref}`eq08` será escrita como $\color{red}{[A \; | \; b]}$.

:::{include} examples.md
:start-after: <!-- Start Exemple 1.16 -->
:end-before: <!-- End Exemple 1.16 -->
:::