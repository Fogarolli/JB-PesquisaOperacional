# Example 01

<!-- Start Exemple 1.1 -->

```{admonition} Exemplo 1.1
:class: examples
O diretor de uma empresa de açaí da região amazônica tem R\$100.000,00 para investir. Como estratégia, ele decidiu diversificar o investimento entre dois tipos de aplicação: compra de equipamentos para processamento de açaí (com retorno estimado de 5% ao ano) e ações de uma cooperativa de produtores da região (com retorno estimado de 9% ao ano). O objetivo do diretor é obter um retorno total de R\$7.800,00 ao ano com esses investimentos. 

Definindo ${x}$ como o valor investido em equipamentos e ${x}$ como o valor investido nas ações da cooperativa, temos as seguintes condições:

1. O total investido deve ser R\$100.000,00:

$$
x + y = 100.000
$$

2. O retorno total esperado deve ser R\$7.800,00:

$$
0,05x + 0,09y = 7.800
$$

Assim, formamos o seguinte sistema linear:

$$
\begin{matrix}
x     & + & y     & = & 100.000 \\ 
0,05x & + & 0,09y & = & 7.800 
\end{matrix} 
$$


Para resolver o sistema, realizamos uma manipulação algébrica que gera um **sistema equivalente**. Multiplicamos a primeira equação por ${-0,05}$ e somamos à segunda, eliminando a variável ${x}$. Isso gera o seguinte sistema equivalente:

$$
\begin{matrix}
x     & + & y     & = & 100.000 \\ 
      &   & 0,04y & = & 2.800 
\end{matrix} 
$$

A partir da nova equação gerada ($0,04y =  2.800$), isolamos ${y}$:

$$
y = 70.000
$$ 

Substituímos o valor de ${y}$ na primeira equação:

$$
x + 70.000 = 100.000
$$

$$
x = 30.000
$$

Com isso, o diretor deve investir R\$30.000 em equipamentos e R\$70.000 nas ações da cooperativa para atingir o retorno esperado de R\$7.800 ao ano. Esses valores satisfazem ambas as equações do sistema linear, garantindo o sucesso da estratégia de investimento.
```
<!-- End Exemple 1.1 -->

# Example 02

<!-- Start Exemple 1.2 -->
````{admonition} Exemplo 1.2
:class: examples

Considera o sistema linear

```{math}
  \begin{align}
    x - 3y = -7 \\
    2x - 6y = 7 
  \end{align}
```
Decidimos novamente eliminar ${x}$. Adicionamos ${(-2)}$ vezes a primeira equação à segunda, obtendo

```{math}
  \begin{align}
    x - 3y = -7 \\
    0x + 0y = 21 
  \end{align}
```

onde a segunda equação não tem sentido. Isto significa que o sistema linear nao tem solução. Poderíamos chegar à mesma conclusão observando que o lado esquerdo da segunda equação é igual ao dobro do lado esquerdo da primeira equação, mas o lado direito da segunda equação não é igual ao dobro do lado direito da primeira equação.
````
<!-- End Exemple 1.2 -->

# Example 03

<!-- Start Exemple 1.3 -->
````{admonition} Exemplo 1.3
:class: examples

Considere o sistema linear

```{math}
  \begin{align}
    x + 2y - 3z &= -4 \\
    2x + y - 3z &= 4 
  \end{align}
```

Para eliminar a variável ${x}$, multiplicamos a primeira equação por ${(-2)}$ e somamos à segunda equação. Essa manipulação gera um **sistema equivalente**:

$$
  \begin{matrix}
    x     & + & 2y & - & 3z & = & -4 \\ 
          & - & 3y & + & 3z & = & 12 
  \end{matrix} 
$$

A partir da equação gerada ($-3y + 3z = 12$), isolamos ${y}$ em função de ${z}$:

$$
  y = z - 4
$$

Substituímos ${y}$ na primeira equação para determinar ${x}$ em função de ${z}$:

$$
  x + 2(z - 4) - 3z = -4
$$

$$
  x = z + 4
$$

Assim, uma solução geral para o sistema é dada por:

$$
  x = r + 4, \\ y = r - 4, \\ z = r
$$

Onde ${r}$ é um número real arbitrário. Isso significa que o sistema tem **infinitas soluções**, dependendo do valor atribuído a ${r}$.

- Se ${r = 1}$:

$$
  x = 5, \\ y = -3, \\ z = 1
$$

- Se ${r = -2}$:

$$
  x = 2, \\ y = -6, \\ z = -2
$$

Cada valor de ${r}$ gera uma solução válida.
````
<!-- End Exemple 1.3 -->

# Example 04

<!-- Start Exemple 1.4 -->

````{admonition} Exemplo 1.4
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
```{dropdown} Análises
- ${A}$ é uma matriz ${2 \times 3}$ com ${a_{11} = 1}$, ${a_{12} = 2}$, ${a_{13} = 3}$, ${a_{21} = 0}$, ${a_{22} = -1}$, ${a_{23} = 0}$.  
- ${B}$ é uma matriz ${2 \times 1}$, com ${b_{11} = 4}$, ${b_{21} = -3}$.   
- ${C}$ é uma matriz ${2 \times 1}$, com ${c_{11} = 1}$, ${c_{21} = 2}$.  
- ${D}$ é uma matriz ${2 \times 2}$, com ${d_{11} = 2}$, ${d_{12} = 0}$, ${d_{21} = -1}$, ${d_{22} = 9}$.  
- ${E}$ é uma matriz ${1 \times 1}$, com ${e_{11} = 3}$.  
- ${F}$ é uma matriz ${2 \times 2}$, em que os elementos ${f_{11} = 1}$ e ${f_{22} = 2}$ formam a diagonal principal.  
```
````

<!-- End Exemple 1.4 -->

# Example 05

<!-- Start Exemple 1.5 -->

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

<!-- End Exemple 1.5 -->

# Example 06

<!-- Start Exemple 1.6 -->

``` {admonition} Exemplo 1.6
:class: examples
São matrizes diagonais:

$$ 
  G = \begin{bmatrix} 4 & 0 \\ 0 & 9 \end{bmatrix} \quad e \quad
  H = \begin{bmatrix} -3 & 0 & 0 \\ 0 & -2 & 0 \\ 0 & 0 & 4 \end{bmatrix}
$$
```

<!-- End Exemple 1.6 -->

# Example 07

<!-- Start Exemple 1.7 -->

``` {admonition} Exemplo 1.7
:class: examples
São matrizes escalares:

$$ 
  G = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{bmatrix} \quad e \quad
  H = \begin{bmatrix} -3 & 0 \\ 0 & -3 \end{bmatrix}
$$
```

<!-- End Exemple 1.7 -->

# Example 08

<!-- Start Exemple 1.8 -->


``` {admonition} Exemplo 1.8
:class: examples
As matrizes

$$
  A = \begin{bmatrix} 1 & 2 & -1 \\ 2 & -3 & 4 \\ 0 & -4 & 5 \end{bmatrix} \quad \text{e} \quad
  B = \begin{bmatrix} 1 & 2 & w \\ 2 & x & 4 \\ y & -4 & z
  \end{bmatrix}
$$

são iguais se ${w = -1}$, ${x = -3}$, ${y = 0}$ e ${z = 5}$.
```

<!-- End Exemple 1.8 -->

# Example 09

<!-- Start Exemple 1.9 -->

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

Deve-se notar que a soma das matrizes ${A}$ e ${B}$ é definida somente quando ${A}$ e ${B}$ têm o mesmo número de linhas e de colunas, isto é, apenas quando ${A}$ e ${B}$ são do mesmo tamanho.
```

<!-- End Exemple 1.9 -->

# Example 10

<!-- Start Exemple 1.10 -->
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
<!-- End Exemple 1.10 -->


# Example 11

<!-- Start Exemple 1.11 -->
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
<!-- End Exemple 1.11 -->

# Example 12

<!-- Start Exemple 1.12 -->
```{admonition} Exemplo 1.12
:class: examples

O produto escalar de: ${u}$ $= \begin{bmatrix} 1 \\ 2 \\ 3 \\ 4 \end{bmatrix}$ e ${v}$ $ = \begin{bmatrix} 2 \\ 3 \\ -2 \\ 1 \end{bmatrix}$ é:

$$\mathbf{u} \cdot \mathbf{v} = (1)(2) + (2)(3) + (3)(-2) + (4)(1) = -6.$$

```
<!-- End Exemple 1.12 -->

# Example 13

<!-- Start Exemple 1.13 -->
```{admonition} Exemplo 1.13
:class: examples

Sejam ${a}$ $ = [x \;\; 2 \;\; 3]$ e ${b}$ $ = \begin{bmatrix} 4 \\ 1 \\ 2 \end{bmatrix}$.  
Se ${a}$  ${\cdot}$ ${b} = -4$, encontre ${x}$.

```{dropdown} Solução
$$
\mathbf{a} \cdot \mathbf{b} = 4x + 2 + 6 = -4 \\
4x + 8 = -4 \\
x = -3.
$$
```
<!-- End Exemple 1.13 -->

# Example 14

<!-- Start Exemple 1.14 -->
```{admonition} Exemplos 1.14
:class: examples

Sejam $A = \begin{bmatrix} 1 & 2 & -1 \\ 3 & 1 & 4 \end{bmatrix} \quad \text{e} \quad B = \begin{bmatrix} -2 & 5 \\ 4 & -3 \\ 2 & 1 \end{bmatrix}.$ Então,

$$
  B = \begin{bmatrix}
    (1)(-2) + (2)(4) + (-1)(2) & (1)(5) + (2)(-3) + (-1)(1) \\
    (3)(-2) + (1)(4) + (4)(2) & (3)(5) + (1)(-3) + (4)(1)
  \end{bmatrix} 
$$
$$
  B = \begin{bmatrix}
    -2 + 8 - 2 & 5 - 6 - 1 \\
    -6 + 4 + 8 & 15 - 3 + 4
  \end{bmatrix} 
  = \begin{bmatrix} 
    4 & -2 \\
    6 & 16
  \end{bmatrix}.
$$
```
<!-- End Exemple 1.14 -->

# Example 15

<!-- Start Exemple 1.15 -->
```{admonition} Exemplos 1.15
:class: examples

O sistema linear

$$
  \begin{aligned}
    x + 2y - z &= 2 \\
    3x \quad\;\;\; + 4z &= 5
  \end{aligned}
$$

pode ser escrito (verifique) utilizando-se o produto matricial a seguir:

$$
  \begin{bmatrix}
    1 & 2 & -1 \\
    3 & 0 &  4
  \end{bmatrix}
  \begin{bmatrix}
    x \\
    y \\
    z
  \end{bmatrix}
    =
  \begin{bmatrix}
    2 \\
    5
  \end{bmatrix}.
$$
```
<!-- End Exemple 1.15 -->

# Example 16

<!-- Start Exemple 1.16 -->

```{admonition} Exemplos 1.16
:class: examples
Considere o sistema linear:

$$
  \begin{aligned}
    -2x + z &= 5 \\
    2x + 3y - 4z &= 7 \\
    3x + 2y + 2z &= 3
  \end{aligned}
$$

Sendo

$$
  A = \begin{bmatrix}
    -2 & 0 & 1 \\
    2 & 3 & -4 \\
    3 & 2 & 2
  \end{bmatrix},
    \quad
  x = \begin{bmatrix}
    x \\
    y \\
    z
  \end{bmatrix},
    \quad
  b = \begin{bmatrix}
    5 \\
    7 \\
    3
  \end{bmatrix},
$$

podemos escrever o sistema linear dado na forma de matriz da seguinte maneira:

$$
  Ax = b.
$$

A matriz de coeficientes é $A$ e a matriz aumentada é:

$$
\left[
  \begin{array}{ccc|c}
    -2 & 0 & 1 & 5 \\
    2 & 3 & -4 & 7 \\
    3 & 2 & 2 & 3
  \end{array}
\right]
$$
```
<!-- End Exemple 1.16 -->


# Example 17

<!-- Start Exemple 1.17 -->

```{admonition} Exemplos 1.17
:class: examples
$$
  F =  \begin{bmatrix} 1 & 2 & 2 & 0 \\ 0 & 1 & 1 & 0 \\ 0 & 0 & 0 & 1 \end{bmatrix} \quad
  G =  \begin{bmatrix} 0 & 2 & -2 & 4 \\ 0 & 0 & 3 & 1 \\ 0 & 0 & 0 & 0 \end{bmatrix} \quad
  H = \begin{bmatrix} 1 & 5 & 0 & 0 & 0 \\ 0 & 1 & 0 & 0 & 0 \\ 0 & 0 & 0 & 0 & 0 \end{bmatrix}
$$

$$
  I = \begin{bmatrix} 0 & 0 & 0 & 1 \\ 0 & 1 & 0 & 0 \\ 1 & 0 & 0 & 0 \\ 0 & 0 & 0 & 0 \end{bmatrix} \quad
  J = \begin{bmatrix} 5 & 7 & 9 \\ 1 & -2 & 3 \\ 0 & 1 & 0 \\ 0 & 0 & 0 \end{bmatrix}
$$
```
<!-- End Exemple 1.17 -->

# Example 18

<!-- Start Exemple 1.18 -->
```{admonition} Exemplos 1.18
:class: examples

Seja

$$
  A = \begin{bmatrix}
    1 & 2 & 4 & 3 \\
    2 & 1 & 3 & 2 \\
    1 & -2 & 2 & 3
  \end{bmatrix}
$$

Se adicionamos 2 vezes a linha 3 de $A$ à segunda linha de $A$, obtemos:

$$
  B = \begin{bmatrix}
    1 & 2 & 4 & 3 \\
    4 & -3 & 7 & 8 \\
    1 & -2 & 2 & 3
  \end{bmatrix}
$$

Portanto, $B$ é equivalente por linhas a $A$.  
Permutando as linhas 2 e 3, obtemos:

$$
  C = \begin{bmatrix}
    1 & 2 & 4 & 3 \\
    1 & -2 & 2 & 3 \\
    4 & -3 & 7 & 8
  \end{bmatrix}
$$

Portanto, $C$ é equivalente por linhas a $B$ e também é equivalente por linhas a $A$.  
Multiplicando a linha 1 de $C$ por 2, obtemos:

$$
  D = \begin{bmatrix}
    2 & 4 & 8 & 6 \\
    1 & -2 & 2 & 3 \\
    4 & -3 & 7 & 8
  \end{bmatrix}
$$

Portanto, $D$ é equivalente por linhas a $C$.  
Segue-se, então, que $D$ é equivalente por linhas a $A$, uma vez que obtivemos $D$ aplicando três operações elementares sucessivas nas linhas de $A$.
```
<!-- End Exemple 1.18 -->



# Example 19

<!-- Start Exemple 1.19 -->
````{admonition} Exemplos 1.19
:class: examples

Seja 

$$
  A = \begin{bmatrix}
    0 & 2 & 3 & -4 & 1\\
    0 & 0 & 2 & 3 & 4 \\
    2 & 2 & -5 & 2 & 4 \\
    2 & 0 & -6 & 9 & 7 \\
  \end{bmatrix}.
$$

O procedimento para a transformação de uma matriz para a forma escalonada por linhas está descrito a seguir.

```{dropdown} Passo 01
Encontre a primeira coluna (da esquerda para a direita) não-nula de $A$. Esta coluna é chamada **coluna do pivô**.

$$
  A = \begin{bmatrix}
    \color{red}{0} & 2 & 3 & -4 & 1\\
    \color{red}{0} & 0 & 2 & 3 & 4 \\
    \color{red}{2} & 2 & -5 & 2 & 4 \\
    \color{red}{2} & 0 & -6 & 9 & 7 \\
  \end{bmatrix}.
$$
```

```{dropdown} Passo 02
Identifique o primeiro elemento não-nulo (de cima para baixo) na coluna do pivô. Este elemento é chamado **pivô**, destacado em azul em $A$.

$$
  A_{1} = \begin{bmatrix}
    \color{red}{0} & 2 & 3 & -4 & 1\\
    \color{red}{0} & 0 & 2 & 3 & 4 \\
    \color{blue}{2} & 2 & -5 & 2 & 4 \\
    \color{red}{2} & 0 & -6 & 9 & 7 \\
  \end{bmatrix}.
$$

```

```{dropdown} Passo 03
Permute, se necessário, a primeira linha com a linha onde está o pivô de modo que o pivô esteja agora na primeira linha. Chame a nova matriz de $A_1$:

$$
  A = \begin{bmatrix}
    \color{blue}{2} & 2 & -5 & 2 & 4 \\
    \color{red}{0} & 0 & 2 & 3 & 4 \\
    \color{red}{0} & 2 & 3 & -4 & 1\\    
    \color{red}{2} & 0 & -6 & 9 & 7 \\
  \end{bmatrix}.
$$


**A primeira e terceira linhas de $A$ foram permutadas.**
```

```{dropdown} Passo 04
Multiplique a primeira linha de $A_1$ pelo inverso do pivô. Dessa maneira, o elemento na primeira linha e coluna do pivô (onde o pivô está localizado) é agora igual a 1. Chame a nova matriz de $A_2$:

$$
  A_{2} = \begin{bmatrix}
    \color{red}{1} & \color{red}{1} & \color{red}{-\frac{5}{2}} & \color{red}{1} & \color{red}{2} \\
    0 & 0 & 2 & 3 & 4 \\
    0 & 2 & 3 & -4 & 1\\
    2 & 0 & -6 & 9 & 7 \\
  \end{bmatrix}.
$$

**A primeira linha de $A_1$ foi multiplicada por $\frac{1}{2}$.**

```

```{dropdown} Passo 05
Adicione múltiplos apropriados da primeira linha de $A_2$ a todas as outras linhas para tornar todos os elementos da coluna do pivô, com exceção do elemento onde o pivô está localizado, iguais a zero. Dessa maneira, todos os elementos na coluna do pivô e linhas $2, 3, \dots, m$ são iguais a zero. Chame a nova matriz de $A_3$:

$$
  A_{3} = \begin{bmatrix}
    1 & 1 & -\frac{5}{2} & 1 & 2 \\
    \color{blue}{0} & 0 & 2 & 3 & 4 \\
    \color{blue}{0} & 2 & 3 & -4 & 1\\
    \color{red}{0} & \color{red}{-2} & \color{red}{-1} & \color{red}{7} & \color{red}{3} \\
  \end{bmatrix}.
$$

**$-2$ vezes a primeira linha de $A_2$ foi adicionada à sua quarta linha.**
```

```{dropdown} Passo 06
Identifique $B$ como a submatriz $(m - 1) \times n$ de $A_3$, obtida retirando-se a primeira linha de $A_3$. Repita os Passos 1 até 5 em $B$:

$$
  B = \begin{bmatrix}
    \color{lightgray}{1} & \color{lightgray}{1} & \color{lightgray}{-\frac{5}{2}} & \color{lightgray}{1} & \color{lightgray}{2} \\
    0 & \color{red}{0} & 2 & 3 & 4 \\
    0 & \color{blue}{2} & 3 & -4 & 1\\
    0 & \color{red}{-2} & -1 & 7 & 3 \\
  \end{bmatrix}.
$$

**A primeira e segunda linhas de $B$ foram permutadas.**

$$
  B_{1} = \begin{bmatrix}
    \color{lightgray}{1} & \color{lightgray}{1} & \color{lightgray}{-\frac{5}{2}} & \color{lightgray}{1} & \color{lightgray}{2} \\
    0 & \color{blue}{2} & 3 & -4 & 1\\
    0 & \color{red}{0} & 2 & 3 & 4 \\
    0 & \color{red}{-2} & -1 & 7 & 3 \\
  \end{bmatrix}.
$$

**A primeira linha de $B_{1}$ foi multiplicada por $\frac{1}{2}$**

$$
  B_{2} = \begin{bmatrix}
    \color{lightgray}{1} & \color{lightgray}{1} & \color{lightgray}{-\frac{5}{2}} & \color{lightgray}{1} & \color{lightgray}{2} \\
    \color{red}{0} & \color{blue}{1} & \color{red}{\frac{3}{2}} & \color{red}{-2} & \color{red}{\frac{1}{2}}\\
    0 & 0 & 2 & 3 & 4 \\
    0 & -2 & -1 & 7 & 3 \\
  \end{bmatrix}.
$$

**$2$ vezes a primeira linha de $B_{2}$ foi adicionada à sua terceira linha**

$$
  B_{3} = \begin{bmatrix}
    \color{lightgray}{1} & \color{lightgray}{1} & \color{lightgray}{-\frac{5}{2}} & \color{lightgray}{1} & \color{lightgray}{2} \\
    0 & 1 & \frac{3}{2} & -2 & \frac{1}{2}\\
    0 & 0 & 2 & 3 & 4 \\
    \color{red}{0} & \color{red}{0} & \color{red}{2} & \color{red}{3} & \color{red}{4} \\
  \end{bmatrix}.
$$

```

```{dropdown} Passo 07
Identifique $C$ como a submatriz $(m - 2) \times n$ de $B_3$, obtida retirando-se a primeira linha de $B_3$. Repita os Passos 1 até 5 em $C$:

$$
  C = \begin{bmatrix}
    \color{lightgray}{1} & \color{lightgray}{1} & \color{lightgray}{-\frac{5}{2}} & \color{lightgray}{1} & \color{lightgray}{2} \\
    \color{lightgray}{0} & \color{lightgray}{1} & \color{lightgray}{\frac{3}{2}} & \color{lightgray}{-2} & \color{lightgray}{\frac{1}{2}}\\
    0 & 0 & \color{blue}{2} & 3 & 4 \\    
    0 & 0 & \color{red}{2} & 3 & 4 \\
  \end{bmatrix}.
$$

**A primeira linha de $C$ foi multiplicada por $\frac{1}{2}$**

$$
  C_{1} = \begin{bmatrix}
    \color{lightgray}{1} & \color{lightgray}{1} & \color{lightgray}{-\frac{5}{2}} & \color{lightgray}{1} & \color{lightgray}{2} \\
    \color{lightgray}{0} & \color{lightgray}{1} & \color{lightgray}{\frac{3}{2}} & \color{lightgray}{-2} & \color{lightgray}{\frac{1}{2}}\\
    \color{red}{0} & \color{red}{0} & \color{red}{1} & \color{red}{\frac{3}{2}} & \color{red}{2} \\    
    0 & 0 & 2 & 3 & 4 \\
  \end{bmatrix}.
$$

**$(-2)$ vezes a primeira linha de $C1$ foi adiciona à sua segunda linha.**

$$
  C_{2} = \begin{bmatrix}
    \color{lightgray}{1} & \color{lightgray}{1} & \color{lightgray}{-\frac{5}{2}} & \color{lightgray}{1} & \color{lightgray}{2} \\
    \color{lightgray}{0} & \color{lightgray}{1} & \color{lightgray}{\frac{3}{2}} & \color{lightgray}{-2} & \color{lightgray}{\frac{1}{2}}\\
    0 & 0 & 1 & \frac{3}{2} & 2 \\    
    \color{red}{0} & \color{red}{0} & \color{red}{0} & \color{red}{0} & \color{red}{0} \\
  \end{bmatrix}.
$$

```

```{dropdown} Passo 08
Identifique $D$ como a submatriz $(m - 3) \times n$ de $C_2$, obtida retirando-se a primeira linha de $C_2$. Tentamos repetir os Passos de 1 até 5 em $D$. 

$$
  D = \begin{bmatrix}
    \color{lightgray}{1} & \color{lightgray}{1} & \color{lightgray}{-\frac{5}{2}} & \color{lightgray}{1} & \color{lightgray}{2} \\
    \color{lightgray}{0} & \color{lightgray}{1} & \color{lightgray}{\frac{3}{2}} & \color{lightgray}{-2} & \color{lightgray}{\frac{1}{2}}\\
    \color{lightgray}{0} & \color{lightgray}{0} & \color{lightgray}{1} & \color{lightgray}{\frac{3}{2}} & \color{lightgray}{2} \\    
    0 & 0 & 0 & 0 & 0 \\
  \end{bmatrix}.
$$

Entretanto, como não há linha do pivô em $D$, concluímos o processo. A matriz, representada por $H$, abrange $D$ e as linhas em cinza acima de $D$, na forma escalonada por linhas.

$$
  H = \begin{bmatrix}
    1 & 1 & -\frac{5}{2} & 1 & 2 \\
    0 & 1 & \frac{3}{2} & -2 & \frac{1}{2}\\
    0 & 0 & 1 & \frac{3}{2} & 2 \\    
    0 & 0 & 0 & 0 & 0 \\
  \end{bmatrix}.
$$

```

```{admonition} Dica!
:class: tip
Quando estivermos realizando os cálculos, muitas vezes é possível evitar frações modificando de maneira apropriada os passos do procedimento.
```

````
<!-- End Exemple 1.19 -->




# Example 20
<!-- Start Exemple 1. -->
<!-- End Exemple 1. -->
# Example 21
<!-- Start Exemple 1. -->
<!-- End Exemple 1. -->
# Example 22
<!-- Start Exemple 1. -->
<!-- End Exemple 1. -->
# Example 23
<!-- Start Exemple 1. -->
<!-- End Exemple 1. -->
# Example 24
<!-- Start Exemple 1. -->
<!-- End Exemple 1. -->
# Example 25
<!-- Start Exemple 1. -->
<!-- End Exemple 1. -->