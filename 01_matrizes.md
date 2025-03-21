# Matrizes

Uma **Matriz** $A_{m\,x\,n}$ é um arranjo retangular de $mn$ números reais (ou complexos) distribuídos em $m$ **linhas** horizontais e $n$ **colunas** verticais.

$$
A = 
\begin{bmatrix}
a_{11} & a_{12} & \cdots & a_{1j} & \cdots & a_{1n} \\
a_{21} & a_{22} & \cdots & a_{2j} & \cdots & a_{2n} \\
\vdots & \vdots & \ddots & \vdots & \ddots & \vdots \\
a_{i1} & a_{i2} & \cdots & a_{ij} & \cdots & a_{in} \\
\vdots & \vdots & \ddots & \vdots & \ddots & \vdots \\
a_{m1} & a_{m2} & \cdots & a_{mj} & \cdots & a_{mn} \\
\end{bmatrix}
$$


**i-ésima linha de A:**  

$$
[ a_{i1}, a_{i2}, \dots, a_{ij}, \dots, a_{in} ]
$$  

**j-ésima coluna de A:**  

$$  
\begin{bmatrix} 
    a_{1j} \\ a_{2j} \\ \vdots \\ a_{ij} \\ \vdots \\ a_{mj} 
\end{bmatrix}
$$   

Podemos descrever a matriz $A$ como tendo $m$ linhas e $n$ colunas, representada na forma $m \times n$. Quando o número de linhas é igual ao número de colunas ($m = n$), dizemos que $A$ é uma matriz quadrada de ordem $n$. Além disso, os elementos $a_{11}$, $a_{22}$, $\dots$, $a_{nn}$ compõem a diagonal principal da matriz $A$. O elemento localizado na linha $i$ e coluna $j$ de $A$ é chamado de elemento $(i,j)$ da matriz $A$ ou i,j-ésimo elemento de $A$ e é comumente representado da seguinte forma: 

$$
A = [a_{ij}]
$$

<!-- ------------------------------------------------------------------------------------------ -->

```{admonition} Exemplo 1.4
:class: examples
Sejam

$$
A = \begin{bmatrix} 1 & 2 & 3 \\ 0 & -1 & 0 \end{bmatrix}, \quad \quad
B = \begin{bmatrix} 4 \\ -3 \end{bmatrix}, \quad \quad
C = \begin{bmatrix} 1 \\ 2 \end{bmatrix}
$$

$$
D = \begin{bmatrix} 2 & 0 \\ -1 & 9 \end{bmatrix}, \quad \quad
E = \begin{bmatrix} 3 \end{bmatrix}, \quad \quad
F = \begin{bmatrix} 1 & 0 \\ 0 & 2 \end{bmatrix}
$$

Então, $A$ é uma matriz $2 \times 3$ com $a_{11} = 1$, $a_{12} = 2$, $a_{13} = 3$, $a_{21} = 0$, $a_{22} = -1$, $a_{23} = 0$. $B$ é uma matriz $2 \times 1$, com $b_{11} = 4$, $b_{21} = -3$. $C$ é uma matriz $2 \times 1$, com $c_{11} = 1$, $c_{21} = 2$. $D$ é uma matriz $2 \times 2$, com $d_{11} = 2 $, $d_{12} = 0 $, $d_{21} = -1$, $d_{22} = 9$. $E$ é uma matriz $1 \times 1$, com $e_{11} = 3$. $F$ é uma matriz $2 \times 2$, em que os elementos $f_{11} = 1$ e $f_{22} = 2$ formam a diagonal principal.
```

<!-- ------------------------------------------------------------------------------------------ -->

```{admonition} Vetores
Uma matriz $1 \times n$ ou $n \times 1$ também é chamada **vetor de dimensão n**.
```

<!-- ------------------------------------------------------------------------------------------ -->

```{admonition} Exemplo 1.5
:class: examples
Considere o sistema linear:

$$
\begin{aligned}
x + 2y &= 10 \\
2x + 2y &= 4 \\
3x + 5y &= 26
\end{aligned}
$$

Ao qual podemos associar as seguintes matrizes:

$$
A = \begin{bmatrix} 1 & 2 \\ 2 & 2 \\ 3 & 5 \end{bmatrix}, \quad
x = \begin{bmatrix} x \\ y \end{bmatrix}, \quad
b = \begin{bmatrix} 10 \\ 4 \\ 26 \end{bmatrix}
$$
```

<!-- ------------------------------------------------------------------------------------------ -->

Uma matriz quadrada $A = [a_{ij}]$ em que todo elemento fora da diagonal principal é zero, isto é, $a_{ij} = 0 \; \text{para } i \neq j$ é chamada **matriz diagonal**.

<!-- ------------------------------------------------------------------------------------------ -->

``` {admonition} Exemplo 1.6
:class: examples
São matrizes diagonais:

$$ 
G = \begin{bmatrix} 4 & 0 \\ 0 & 9 \end{bmatrix} \quad e \quad
H = \begin{bmatrix} -3 & 0 & 0 \\ 0 & -2 & 0 \\ 0 & 0 & 4 \end{bmatrix}
$$
```

<!-- ------------------------------------------------------------------------------------------ -->

Uma matriz diagonal $A = [a_{ij}]$ em que todos os termos da diagonal principal são iguais, isto é, $a_{ij} = c \quad \text{para } i = j$ é chamada **matriz escalar**.

<!-- ------------------------------------------------------------------------------------------ -->

``` {admonition} Exemplo 1.7
:class: examples
São matrizes escalares:

$$ 
G = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{bmatrix} \quad e \quad
H = \begin{bmatrix} -3 & 0 \\ 0 & -3 \end{bmatrix}
$$
```

<!-- ------------------------------------------------------------------------------------------ -->


Duas matrizes $m \times n$, $A = [a_{ij}]$ e $B = [b_{ij}]$ são ditas **iguais** se $a_{ij} = b_{ij}, \; 1 \leq i \leq m, 1 \leq j \leq n$, isto é, se os elementos correspondentes forem iguais.

<!-- ------------------------------------------------------------------------------------------ -->

``` {admonition} Exemplo 1.8
:class: examples
As matrizes

$$
A = \begin{bmatrix} 1 & 2 & -1 \\ 2 & -3 & 4 \\ 0 & -4 & 5 \end{bmatrix} \quad \text{e} \quad
B = \begin{bmatrix} 1 & 2 & w \\ 2 & x & 4 \\ y & -4 & z
\end{bmatrix}
$$

são iguais se $w = -1$, $x = -3$, $y = 0$ e $z = 5$.
```

<!-- ------------------------------------------------------------------------------------------ -->

## Adiação de Matrizes 

Se $A = [a_{ij}]$ e $B = [b_{ij}]$ são matrizes $m \times n$, então a **soma** de $A$ e $B$ é a matriz $C = [c_{ij}]$, $m \times n$, definida por

$$
c_{ij} = a_{ij} + b_{ij}, \quad (1 \leq i \leq m, 1 \leq j \leq n).
$$

Portanto, $C$ é obtida pela adição dos elementos correspondentes de $A$ e $B$.

<!-- ------------------------------------------------------------------------------------------ -->

```{admonition} Exemplo 1.9
:class: examples
Sejam

$$
A = \begin{bmatrix} 1 & -2 & 4 \\ 2 & -1 & 3 \end{bmatrix} \quad \text{e} \quad
B = \begin{bmatrix} 0 & 2 & -4 \\ 1 & 3 & 1 \end{bmatrix}
$$

Então,

$$
A + B = \begin{bmatrix} 1 + 0 & -2 + 2 & 4 + (-4) \\ 2 + 1 & -1 + 3 & 3 + 1 \end{bmatrix} = \begin{bmatrix} 1 & 0 & 0 \\ 3 & 2 & 4 \end{bmatrix}.
$$

Deve-se notar que a soma das matrizes $A$ e $B$ é definida somente quando $A$ e $B$ têm o mesmo número de linhas e de colunas, isto é, apenas quando $A$ e $B$ são do mesmo tamanho.
```

<!-- ------------------------------------------------------------------------------------------ -->

```{admonition} Nota
**Devemos agora definir a convenção de que quando $A + B$ é formada, ambas $A$ e $B$ são do mesmo tamanho.**
```

<!-- ------------------------------------------------------------------------------------------ -->

## Multiplicação por um Escalar

Se $A = [a_{ij}]$ é uma matriz $m \times n$ e $r$ é um número real, então a **multiplicação por um escalar** de $A$ por $r$, $rA$, é a matriz $B = [b_{ij}]$, $m \times n$, onde

$$
b_{ij} = r a_{ij} \quad (1 \leq i \leq m, 1 \leq j \leq n).
$$

Então, $B$ é obtida pela multiplicação de cada elemento de $A$ por $r$. Se $A$ e $B$ são matrizes $m \times n$, escrevemos $A + (-1)B$ como $A - B$ e chamamos isto de **diferença de $A$ e $B$**.

<!-- ------------------------------------------------------------------------------------------ -->

```{admonition} Exemplo 1.10
:class: examples
Sejam

$$
A = \begin{bmatrix} 2 & 3 & -5 \\ 4 & 2 & 1 \end{bmatrix} \quad \text{e} \quad 
B = \begin{bmatrix} 2 & -1 & 3 \\ 3 & 5 & -2 \end{bmatrix}.
$$

Então,

$$
A - B = \begin{bmatrix} 2 - 2 & 3 + 1 & -5 - 3 \\ 4 - 3 & 2 - 5 & 1 + 2 \end{bmatrix} = 
\begin{bmatrix} 0 & 4 & -8 \\ 1 & -3 & 3 \end{bmatrix} 
$$
```

<!-- ------------------------------------------------------------------------------------------ -->

Se $A_1, A_2, \dots, A_k$ são matrizes $m \times n$ e $c_1, c_2, \dots, c_k$ são números reais, então uma expressão do tipo

$$
c_1 A_1 + c_2 A_2 + \dots + c_k A_k
$$

é chamada **combinação linear** de $A_1, A_2, \dots, A_k$, e $c_1, c_2, \dots, c_k$ são denominados **coeficientes da combinação**.

<!-- ------------------------------------------------------------------------------------------ -->

## A Transposta de uma Matriz

Se $A = [a_{ij}]$ é uma matriz $m \times n$, então a matriz $n \times m$, $A^T = [a_{ji}]$, onde

$$
a^T_{ij} = a_{ji} \quad (1 \leq i \leq n, 1 \leq j \leq m),
$$

é chamada **transposta** de $A$. Dessa maneira, os elementos em cada linha de $A^T$ são os elementos na coluna correspondente de $A$.

<!-- ------------------------------------------------------------------------------------------ -->

```{admonition} Exemplo 1.11
:class: examples
Sejam

$$
A = \begin{bmatrix} 4 & -2 & 3 \\ 0 & 5 & -2 \end{bmatrix}, \quad 
B = \begin{bmatrix} 6 & 2 & 4 \\ 0 & 4 & 3 \end{bmatrix},
$$

$$
C = \begin{bmatrix} 5 & -3 & 2 \\ 4 & 2 & -3 \end{bmatrix}, \quad 
D = \begin{bmatrix} 3 & -5 & 1 \end{bmatrix}, \quad 
E^T = \begin{bmatrix} 2 \\ -1 \\ 3 \end{bmatrix}.
$$

Então,

$$
A^T = \begin{bmatrix} 4 & 0 \\ -2 & 5 \\ 3 & -2 \end{bmatrix}, \quad 
B^T = \begin{bmatrix} 6 & 0 \\ 2 & 4 \\ 4 & 3 \end{bmatrix},
$$

$$
C^T = \begin{bmatrix} 5 & 4 \\ -3 & 2 \\ 2 & -3 \end{bmatrix}, \quad 
D^T = \begin{bmatrix} 3 \\ -5 \\ 1 \end{bmatrix}, \quad 
E^T = \begin{bmatrix} 2 & -1 & 3 \end{bmatrix}.
$$
```

<!-- ------------------------------------------------------------------------------------------ -->

```{admonition} Exercício 1.3 - Produção
:class: exercise
Um fabricante de um determinado produto produz três modelos A, B e C. Cada modelo é produzido parcialmente na fábrica $F_1$ em Macapá e, então, finalizado na fábrica $F_2$ Santana. O custo total de cada produto é composto pelo custo de produção e pelo custo de transporte. Portanto, o custo de cada fábrica, em reais, pode ser descrito pelas matrizes $F_1$ e $F_2$, $3 \times 2$:

$$
\begin{array}{c|cc}
& \text{Custo de} & \text{Custo de} \\
F1 & \text{Produção} & \text{Transporte} \\
\hline
\text{Modelo A} & 32 & 40 \\
\text{Modelo B} & 50 & 80 \\
\text{Modelo C} & 70 & 20
\end{array}
$$

$$
\begin{array}{c|cc}
& \text{Custo de} & \text{Custo de} \\
F2 & \text{Produção} & \text{Transporte} \\
\hline
\text{Modelo A} & 40 & 60 \\
\text{Modelo B} & 50 & 50 \\
\text{Modelo C} & 130 & 20
\end{array}
$$

A matriz $F_1 + F_2$ fornece o total dos custos de produção e transporte para cada produto. Assim, qual é o total dos custos de produção e transporte para um produto do modelo C?
```

<!-- ------------------------------------------------------------------------------------------ -->

```{admonition} Exercício 1.4
:class: exercise

Seja $p = [18.95, 14.75, 8.60]$ um vetor de dimensão 3 que representa os preços atuais de três itens de uma loja. Suponha que a loja anuncie uma promoção em que o preço de cada item esteja reduzido em 20%.

(a) Determine um vetor de dimensão 3 que forneça as alterações de preço para os três itens.  
(b) Determine um vetor de dimensão 3 que forneça os novos preços dos itens.
```

<!-- ------------------------------------------------------------------------------------------ -->

```{admonition} Exercício 1.5
:class: exercise

Se 

$$
A_1 = \begin{bmatrix} 0 & -3 & 5 \\ 2 & 3 & 4 \\ 1 & -2 & -3 \end{bmatrix} \quad \text{e} \quad
A_2 = \begin{bmatrix} 5 & 2 & 3 \\ 6 & 2 & 3 \\ -1 & -2 & 3 \end{bmatrix}
$$

então $C = 3A_1 - \frac{1}{2} A_2$ é uma combinação linear de $A_1$ e $A_2$. 

(a) Utilizando a multiplicação escalar e a adição de matriz, calcule $C.

(b) $ 2 \begin{bmatrix} 3 & -2 \end{bmatrix} - 3 \begin{bmatrix} 5 & 0 \end{bmatrix} + 4 \begin{bmatrix} -2 & 5 \end{bmatrix} $ é uma combinação linear de $\begin{bmatrix} 3 & -2 \end{bmatrix}$, $\begin{bmatrix} 5 & 0 \end{bmatrix}$ e $\begin{bmatrix} -2 & 5 \end{bmatrix}$. Isto pode ser calculado (verifique) como $\begin{bmatrix} -17 & 16\end{bmatrix}$.

(c) $ -0.5\begin{bmatrix} 1 \\ -4 \\ -6 \end{bmatrix} + 0.4 \begin{bmatrix} 0.1 \\ -4 \\ 0.2 \end{bmatrix}$ é uma combinação linear de $\begin{bmatrix} 1 \\ -4 \\ -6 \end{bmatrix} $ e $\begin{bmatrix} 0.1 \\ -4 \\ 0.2 \end{bmatrix}$. Isto pode ser calculado (verifique) como $\begin{bmatrix} -0.46 \\ 0.4 \\ 3.08 \end{bmatrix}$.
```








