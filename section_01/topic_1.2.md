# Matrizes

Uma **Matriz** $\color{red}{A_{m\,x\,n}}$ é um arranjo retangular de $\color{red}{mn}$ números reais (ou complexos) distribuídos em $\color{red}{m}$ **linhas** horizontais e $\color{red}{n}$ **colunas** verticais.

$$
    A = \begin{bmatrix}
            a_{11} & a_{12} & \cdots & \color{red}{\mathbf{a_{1j}}} & \cdots & a_{1n} \\
            a_{21} & a_{22} & \cdots & \color{red}{\mathbf{a_{2j}}} & \cdots & a_{2n} \\
            \vdots & \vdots & \ddots & \color{red}{\mathbf{\vdots}} & \ddots & \vdots \\
            \color{red}{\mathbf{a_{i1}}} & \color{red}{\mathbf{a_{i2}}} & \color{red}{\mathbf{\cdots}} & \color{red}{\mathbf{a_{ij}}} & \color{red}{\mathbf{\cdots}} & \color{red}{\mathbf{a_{in}}} \\
            \vdots & \vdots & \ddots & \color{red}{\mathbf{\vdots}} & \ddots & \vdots \\
            a_{m1} & a_{m2} & \cdots & \color{red}{\mathbf{a_{mj}}} & \cdots & a_{mn} \\
        \end{bmatrix}
$$

**i-ésima linha de A:** 

$$ 
    \begin{bmatrix} 
    \; \color{red}{a_{i1}} & \color{red}{a_{i2}} & \color{red}{\dots} & \color{red}{a_{ij}} & \color{red}{\dots} & \color{red}{a_{in}} \;
    \end{bmatrix}
$$

**j-ésima coluna de A:**  

$$  
\begin{bmatrix} 
    \color{red}{a_{1j}} \\ \color{red}{a_{2j}} \\ \color{red}{\vdots} \\ \color{red}{a_{ij}} \\ \color{red}{\vdots} \\ \color{red}{a_{mj}} 
\end{bmatrix}
$$   

Podemos descrever a **matriz $\color{red}{A}$** como tendo **$\color{red}{m}$ linhas** e **$\color{red}{n}$ colunas**, representada na forma $\color{red}{m \times n}$. Quando o número de linhas é igual ao número de colunas ($\color{red}{m = n}$), dizemos que $A$ é uma **matriz quadrada de ordem $\color{red}{n}$**. Além disso, os elementos $\color{red}{a_{11}}$, $\color{red}{a_{22}}$, $\color{red}{\dots}$, $\color{red}{a_{nn}}$ compõem a **diagonal principal da matriz $\color{red}{A}$**. O elemento localizado na linha $\color{red}{i}$ e coluna $\color{red}{j}$ de $\color{red}{A}$ é chamado de elemento $\color{red}{(i,j)}$ da matriz $\color{red}{A}$ ou **i,j-ésimo** elemento de $\color{red}{A}$ e é comumente representado da seguinte forma: 

$$
    A = [a_{ij}]
$$


👉 Uma matriz quadrada $\color{red}{A = [a_{ij}]}$ em que todo elemento fora da diagonal principal é **zero**, isto é, $\color{red}{a_{ij} = 0}$ para $\color{red}{i \neq j}$ é chamada **matriz diagonal**.

👉 Uma matriz diagonal $\color{red}{A = [a_{ij}]}$ em que todos os termos da diagonal principal são iguais, isto é, $\color{red}{a_{ij} = c}$ para $\color{red}{i = j}$ é chamada **matriz escalar**.

👉 Duas matrizes $\color{red}{m \times n}$, $\color{red}{A = [a_{ij}]}$ e $\color{red}{B = [b_{ij}]}$ são ditas **iguais** se $\color{red}{a_{ij} = b_{ij}, \; 1 \leq i \leq m, 1 \leq j \leq n}$, isto é, se os elementos correspondentes forem **iguais**.

```{admonition} Vetores
Uma matriz $1 \times n$ ou $n \times 1$ também é chamada **vetor de dimensão n**.
```

:::{include} examples.md
:start-after: <!-- Start Exemple 1.4 -->
:end-before: <!-- End Exemple 1.4 -->
:::

:::{include} examples.md
:start-after: <!-- Start Exemple 1.5 -->
:end-before: <!-- End Exemple 1.5 -->
:::

:::{include} examples.md
:start-after: <!-- Start Exemple 1.6 -->
:end-before: <!-- End Exemple 1.6 -->
:::

:::{include} examples.md
:start-after: <!-- Start Exemple 1.7 -->
:end-before: <!-- End Exemple 1.7 -->
:::

:::{include} examples.md
:start-after: <!-- Start Exemple 1.8 -->
:end-before: <!-- End Exemple 1.8 -->
:::

:::{include} examples.md
:start-after: <!-- Start Exemple 1.9 -->
:end-before: <!-- End Exemple 1.9 -->
:::

## Adiação de Matrizes 

Se $\color{red}{A = [a_{ij}]}$ e $\color{red}{B = [b_{ij}]}$ são matrizes $\color{red}{m \times n}$, então a **soma** de $\color{red}{A}$ e $\color{red}{B}$ é a matriz $\color{red}{C = [c_{ij}]}$, $\color{red}{m \times n}$, definida por

```{math}
:label: eq03
    c_{ij} = a_{ij} + b_{ij}, \quad (1 \leq i \leq m, 1 \leq j \leq n).
```

Portanto, $\color{red}{C}$ é obtida pela adição dos elementos correspondentes de $\color{red}{A}$ e $\color{red}{B}$.

```{admonition} Atenção!
:class: warning
**Devemos agora definir a convenção de que quando $\color{red}{A + B}$ é formada, ambas $\color{red}{A}$ e $\color{red}{B}$ são do mesmo tamanho.**
```

## Multiplicação por um Escalar

Se $\color{red}{A = [a_{ij}]}$ é uma matriz $\color{red}{m \times n}$ e $\color{red}{r}$ é um número real, então a **multiplicação por um escalar** de $\color{red}{A}$ por $\color{red}{r}$, $\color{red}{rA}$, é a matriz $\color{red}{B = [b_{ij}]}$, $\color{red}{m \times n}$, onde

```{math}
:label: eq04
    b_{ij} = r a_{ij} \quad (1 \leq i \leq m, 1 \leq j \leq n).
```

Então, $\color{red}{B}$ é obtida pela multiplicação de cada elemento de $\color{red}{A}$ por $\color{red}{r}$. 

```{admonition} Nota!
Se $\color{red}{A}$ e $\color{red}{B}$ são matrizes $\color{red}{m \times n}$, escrevemos $\color{red}{A + (-1)B}$ como $\color{red}{A - B}$ e chamamos isto de **diferença de $\color{red}{A}$ e $\color{red}{B}$**.
```

:::{include} examples.md
:start-after: <!-- Start Exemple 1.10 -->
:end-before: <!-- End Exemple 1.10 -->
:::


Se $\color{red}{A_1}$, $\color{red}{A_2}$, $\color{red}{\dots}$, $\color{red}{A_k}$ são matrizes $\color{red}{m \times n}$ e $\color{red}{c_1}$, $\color{red}{c_2}$, $\color{red}{\dots}$, $\color{red}{c_k}$ são números reais, então uma expressão do tipo

$$
    c_1 A_1 + c_2 A_2 + \dots + c_k A_k
$$

é chamada **combinação linear** de $\color{red}{A_1}$, $\color{red}{A_2}$, $\color{red}{\dots}$, $\color{red}{A_k}$, e $\color{red}{c_1}$, $\color{red}{c_2}$, $\color{red}{\dots}$, $\color{red}{c_k}$ são denominados **coeficientes da combinação**.


## A Transposta de uma Matriz

Se $\color{red}{A = [a_{ij}]}$ é uma matriz $\color{red}{m \times n}$, então a matriz $\color{red}{n \times m}$, $\color{red}{A^T = [a_{ji}]}$, onde

```{math}
:label: eq05
    a^T_{ij} = a_{ji} \quad (1 \leq i \leq n, 1 \leq j \leq m),
```

é chamada **transposta** de $\color{red}{A}$. Dessa maneira, os elementos em cada linha de $\color{red}{A^T}$ são os elementos na coluna correspondente de $\color{red}$.

:::{include} examples.md
:start-after: <!-- Start Exemple 1.11 -->
:end-before: <!-- End Exemple 1.11 -->
:::
