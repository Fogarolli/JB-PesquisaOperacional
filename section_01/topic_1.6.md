# Eliminação de Gauss-Jordan

Nesta seção, vamos organizar o processo de eliminação utilizado na resolução de sistemas lineares, como discutido anteriormente. O objetivo é desenvolver um método prático e eficiente para encontrar soluções desses sistemas. Esse método começa com a **matriz aumentada** associada ao sistema linear e aplica transformações que a convertem em uma forma mais simples. Essa nova forma mantém as mesmas soluções do sistema original, mas facilita significativamente o processo de resolução. Por exemplo, considere a seguinte matriz aumentada:


$$
    \left[
        \begin{array}{cccc|c}
            1 & 0 & 0 & 2 & 4 \\
            0 & 1 & 0 & -1 & -5 \\
            0 & 0 & 1 & 3 & 6
        \end{array}
    \right]
$$

Essa matriz corresponde ao seguinte sistema de equações:

$$
    \begin{aligned}
        x_1 + 2x_4 & = 4 \\
        x_2 - x_4 & = -5 \\
        x_3 + 3x_4 & = 6
    \end{aligned}
$$

Como as equações já estão isoladas nas variáveis $\color{red}{x_1}$, $\color{red}{x_2}$ e $\color{red}{x_3}$, é fácil encontrar suas soluções em função de $\color{red}{x_4}$. O principal objetivo desta seção é aprender a manipular qualquer matriz aumentada até atingir uma forma semelhante a essa, na qual as soluções possam ser encontradas de maneira simples e direta.

## Forma Escalonada Reduzida por Linhas

Uma matriz $\color{red}{m \times n}$ está na **forma escalonada reduzida por linhas** se ela satisfaz as seguintes propriedades:

- **(a)** Todas as linhas nulas, se existirem, ocorrem abaixo de todas as linhas não-nulas.  
- **(b)** O primeiro elemento diferente de zero à partir da esquerda de uma linha diferente de zero é um 1. Este elemento é chamado de **um inicial** desta linha.  
- **(c)** Para cada linha diferente de zero, um inicial aparece à direita dos uns iniciais das linhas precedentes.  
- **(d)** Se uma coluna contém um inicial, então todos os outros elementos naquela coluna são iguais a zero.

Em uma matriz na **forma escalonada reduzida por linhas**, os primeiros coeficientes das linhas não-nulas formam uma escada. Uma matriz $\color{red}{m \times n}$ que satisfaz as propriedades (a), (b) e (c) está na **forma escalonada por linhas**. As matrizes a seguir estão na **forma escalonada por linhas**:

:::{include} examples.md
:start-after: <!-- Start Exemple 1.17 -->
:end-before: <!-- End Exemple 1.17 -->
:::

Agora que já entendemos o que caracteriza uma matriz na **forma escalonada reduzida por linhas**, vamos avançar e aprender **como transformar qualquer matriz em sua forma escalonada por linhas**. A partir dessa forma intermediária, será possível alcançar a forma reduzida com alguns passos adicionais. 

Esse processo é essencial para resolver sistemas lineares de maneira organizada e eficiente, utilizando um conjunto de procedimentos bem definidos. Para isso, utilizaremos as chamadas **operações elementares nas linhas** de uma matriz $\color{red}{A = [a_{ij}], \, m \times n}$, que podem ser de três tipos:

- **(a)** **Permutação** de duas linhas de $\color{red}{A}$. Ou seja, substitua $\color{red}{a_{r1}}$, $\color{red}{a_{r2}}$, $\color{red}{\ldots}$, $\color{red}{a_{rn}}$ por $\color{red}{a_{s1}}$, $\color{red}{a_{s2}}$, $\color{red}{\ldots}$, $\color{red}{a_{sn}}$ e vice-versa, onde $\color{red}{r \neq s}$.

- **(b)** **Multiplicação** de uma linha de $\color{red}{A}$ por um número constante diferente de zero $\color{red}{c}$. Ou seja, substitua $\color{red}{a_{r1}}$, $\color{red}{a_{r2}}$, $\color{red}{\ldots}$, $\color{red}{a_{rn}}$ por $\color{red}{ca_{r1}}$, $\color{red}{ca_{r2}}$, $\color{red}{\ldots}$, $\color{red}{ca_{rn}}$.

- **(c)** **Adição** de um múltiplo de uma linha a outra linha. Ou seja, substitua a linha $\color{red}{r}$ por ela mesma somada a $\color{red}{d}$ vezes a linha $\color{red}{s}$, com $\color{red}{r \neq s}$: $\color{red}{a_{r1}}$, $\color{red}{a_{r2}}$, $\color{red}{\ldots}$, $\color{red}{a_{rn}}$ por $\color{red}{a_{r1}}$ $\color{red}{+  \; da_{s1}}$, $\color{red}{a_{r2}}$ $\color{red}{+ \; da_{s2}}$, $\color{red}{\ldots}$,$\color{red}{ a_{rn}}$ $\color{red}{+  \; da_{sn}}$.


```{admonition} Atenção!
:class: warning
Quando uma matriz é vista como a matriz aumentada de um sistema linear, essas operações correspondem a operações válidas feitas nas equações do sistema:

- permutar equações,
- multiplicar uma equação por uma constante não nula,
- somar um múltiplo de uma equação a outra.

Essas operações **não alteram as soluções do sistema**.
```

Uma matriz $\color{red}{A \, m \times n}$ é **equivalente por linhas** a uma matriz $\color{red}{B \, m \times n}$ se $\color{red}{B}$ pode ser obtida aplicando-se uma sequência finita de operações elementares nas linhas da matriz $\color{red}{A}$.

:::{include} examples.md
:start-after: <!-- Start Exemple 1.18 -->
:end-before: <!-- End Exemple 1.18 -->
:::
 
```{admonition} Nota!

Não é difícil mostrar que:

1. Toda matriz é equivalente por linhas a si mesma;  
2. Se $A$ é equivalente por linhas a $B$, então $B$ é equivalente por linhas a $A$;  
3. Se $A$ é equivalente por linhas a $B$ e $B$ é equivalente por linhas a $C$, então $A$ é equivalente por linhas a $C$.

Em 2, as afirmações “$A$ é equivalente por linhas a $B$” e “$B$ é equivalente por linhas a $A$” podem ser substituídas por **“$A$ e $B$ são equivalentes por linhas”**.
```

:::{include} examples.md
:start-after: <!-- Start Exemple 1.19 -->
:end-before: <!-- End Exemple 1.19 -->
:::