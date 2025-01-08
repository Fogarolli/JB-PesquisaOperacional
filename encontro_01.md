# Álgebra Linear

Neste capítulo, faremos uma revisão dos conceitos fundamentais sobre sistemas lineares e matrizes, que servirão como base para o estudo da Pesquisa Operacional.
Os sistemas de equações lineares e as matrizes são pilares importantes na resolução de problemas matemáticos e na modelagem de situações do mundo real, sendo 
amplamente utilizados em áreas como engenharia, economia, computação e ciências aplicadas. A compreensão desses tópicos é essencial, pois muitas das técnicas e 
métodos utilizados nesta disciplina dependem de operações matriciais e da resolução de sistemas de equações lineares.

Revisaremos os métodos para resolução de sistemas lineares, como substituição, adição e eliminação de Gauss, além de operações com matrizes, como multiplicação, 
cálculo de determinantes e inversão de matrizes. Também abordaremos conceitos importantes, como a consistência de sistemas e a singularidade de matrizes, que 
frequentemente aparecem em problemas de otimização e modelagem.

Este capítulo não tem o objetivo de introduzir novos conteúdos, mas sim de consolidar o conhecimento prévio necessário para que possamos explorar os métodos da 
Pesquisa Operacional com maior profundidade. Por meio de exemplos e exercícios, reforçaremos os fundamentos matemáticos que serão utilizados ao longo da disciplina, 
garantindo um aprendizado mais fluido e eficaz.

## Sistemas Lineares

Uma equação do tipo $ax = b$, que expressa a variável $b$ em função da  variável $x$ e da constante $a$, é chamada de **equação linear**. O termo *linear* é 
utilizado porque o gráfico dessa equação é uma linha reta, conforme ilustrado a seguir.

<iframe src="/Users/rafaelvieira/Documents/03_codigos/JB-PesquisaOperacional/imgs/plot.html" width="100%" height="510px" frameborder="0"></iframe>


Da mesma forma, a equação

```{math}
:label: eq01
a_1 x_1 + a_2 x_2 + \cdots + a_n x_n = b,
```

que expressa a variável $b$ em função das variáveis $x_1$, $x_2$, $\cdots$, $x_n$ e das constantes conhecidas $a_1$, $a_2$, $\cdots$, $a_n$ é chamada de equação 
linear. Em diversos cenários, fornecemos $b$ e as constantes $a_1$, $a_2$, $\cdots$, $a_n$ e devemos encontrar os números $x_1$, $x_2$, $\cdots$ , $x_n$ chamados 
**incógnitas**, que satisfazem a equação.

Uma solução de uma equação linear {math:numref}`eq01` é uma sequência de $n$ números $s_1$, $s_2$, $\cdots$, $s_n$ que têm como propriedade satisfazer a expressão 
{math:numref}`eq01` quando $x_1 = s_2$, $x_2 = s_2$, $\cdots$ , $x_n = s_n$ são substituídas nessa expressão. Então, $x_1 = 4$, $x_2 = -1$ e $x_3 = 2$ é uma solução 
para a equação linear:

$$
2x_1 - 3x_2 + 4x_3 = 19,
$$ 

pois 

$$
2(4)- 3(-1) + 4(2) = 19.
$$

Um sistema de **$m$ equações lineares a $n$ incógnitas $x_1$, $x_2$, $\cdots$ , $x_n$** ou simplesmente um **sistema linear**, é um conjunto de $m$ equações lineares,
cada uma com $n$ incógnitas.

```{math}
:label: eq02
\begin{matrix}
a_{11}x_{1} & + & a_{12}x_{2} & + & \cdots & + & a_{1n}x_{n} & = & b_{1} \\
a_{21}x_{1} & + & a_{22}x_{2} & + & \cdots & + & a_{2n}x_{n} & = & b_{2} \\
\vdots      &   & \vdots      &   &        &   & \vdots      &   & \vdots  \\
a_{m1}x_{1} & + & a_{m2}x_{2} & + & \cdots & + & a_{mn}x_{n} & = & b_{m} \\
\end{matrix}
```

Uma **solução** de um sistema linear é uma sequência de $n$ números $s_1$, $s_2$, $\cdots$, $s_n$ que têm como propriedade o fato de satisfazer cada equação do 
sistema quando $x_1 = s_1$, $x_2 = s_2$, $\cdots$ , $x_n = s_n$ são substituídos na expressão. Para resolver um sistema linear, utilizamos uma técnica conhecida 
como **método da eliminação**.

### Método de Eliminação

O método de eliminação é uma técnica utilizada para resolver sistemas lineares. O objetivo principal do método é simplificar o sistema até que as soluções possam ser facilmente determinadas, eliminando variáveis gradualmente. O método de eliminação pode ser resumido nos seguintes passos:

```
  1. Trocar a posição de duas equações.
  2. Multiplicar uma equação por uma constante diferente de zero.
  3. Adicionar um múltiplo de uma equação à outra.
```

O método da eliminação produz outro sistema linear que tem exatamente as mesmas soluções do sistema dado. O novo sistema linear pode, então, ser resolvido facilmente.



````{dropdown} Exemplo 01

  O diretor de uma empresa de açaí da região amazônica tem R\$100.000,00 para investir. Como estratégia, ele decidiu diversificar o investimento entre dois tipos de 
  aplicação: compra de equipamentos para processamento de açaí (com retorno estimado de 5% ao ano) e ações de uma cooperativa de produtores da região (com retorno 
  estimado de 9% ao ano). O objetivo do diretor é obter um retorno total de R\$7.800,00 ao ano com esses investimentos. 

  Definindo **x** como o valor investido em equipamentos e **y** como o valor investido nas ações da cooperativa, temos as seguintes condições:

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


  Para resolver o sistema, realizamos uma manipulação algébrica que gera um **sistema equivalente**. 
  Multiplicamos a primeira equação por **$-0,05$** e somamos à segunda, eliminando a variável **x**. Isso gera o seguinte sistema equivalente:

  $$
  \begin{matrix}
  x     & + & y     & = & 100.000 \\ 
        &   & 0,04y & = & 2.800 
  \end{matrix} 
  $$

  A partir da nova equação gerada ($0,04y =  2.800$), isolamos **y**:

  $$
  y = 70.000
  $$ 

  Substituímos o valor de **y** na primeira equação:

  $$
  x + 70.000 = 100.000
  $$

  $$
  x = 30.000
  $$

  Com isso, o diretor deve investir R\$30.000 em equipamentos e R\$70.000 nas ações da cooperativa para atingir o retorno esperado de R\$7.800 ao ano. 
  Esses valores satisfazem ambas as equações do sistema linear, garantindo o sucesso da estratégia de investimento.

````


````{dropdown} Exemplo 02
  Considera o sistema linear

  ```{math}
  \begin{align}
  x - 3y = -7 \\
  2x - 6y = 7 
  \end{align}
  ```
  Decidimos novamente eliminar $x$. Adicionamos (-2) vezes a primeira equação à segunda, obtendo

  ```{math}
  \begin{align}
  x - 3y = -7 \\
  0x + 0y = 21 
  \end{align}
  ```

  onde a segunda equação não tem sentido. Isto significa que o sistema linear nao tem solução. Poderíamos chegar à mesma conclusão observando que o lado esquerdo da segunda equação é igual ao dobro do lado esquerdo da primeira equação, mas o lado direito da segunda equação não é igual ao dobro do lado direito da primeira equação.

````


````{dropdown} Exemplo 03
  Considere o sistema linear

  ```{math}
  \begin{align}
  x + 2y - 3z &= -4 \\
  2x + y - 3z &= 4 
  \end{align}
  ```

  Para eliminar a variável **x**, multiplicamos a primeira equação por **-2** e somamos à segunda equação. Essa manipulação gera um **sistema equivalente**:

  $$
  \begin{matrix}
  x     & + & 2y & - & 3z & = & -4 \\ 
        & - & 3y & + & 3z & = & 12 
  \end{matrix} 
  $$

  A partir da equação gerada ($-3y + 3z = 12$), isolamos **y** em função de **z**:

  $$
  y = z - 4
  $$

  Substituímos **y** na primeira equação para determinar **x** em função de **z**:

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

  Onde **r** é um número real arbitrário. Isso significa que o sistema tem **infinitas soluções**, dependendo do valor atribuído a **r**.

  - Se **r = 1**:

    $$
    x = 5, \\ y = -3, \\ z = 1
    $$

  - Se **r = -2**:
  
    $$
    x = 2, \\ y = -6, \\ z = -2
    $$

  Cada valor de **r** gera uma solução válida.
````


```{admonition} Nota
Os exemlos apresentados sugerem que um sistemas linear pode ter **uma única solução**, **nenhuma solução**, ou **infinitas soluções**.
```

--- 

<iframe src="/Users/rafaelvieira/Documents/03_codigos/JB-PesquisaOperacional/imgs/grafico_sistemas_lineares.html" width="100%" height="510px" frameborder="0"></iframe>

---

01. O sistema tem uma única solução; ou seja, as retas azul e vermelha se cruzam exatamente em um ponto.
02. O sistema não tem solução; ou seja, as relas azul e vermelha não se cruzam.
03. O sistema tem infinitas soluções, ou seja, as retas azul e vermelha são coincidentes.

---

## Matrizes

Uma **Matriz** $A_{m\,x\,n}$ é um arranjo retangular de $mn$ números reais (ou complexos) distribuídos em $m$ **linhas** horizontais e $n$ **colunas** verticais.

$$
\text{A matriz } A = 
\begin{bmatrix}
a_{11} & a_{12} & \cdots & a_{1j} & \cdots & a_{1n} \\
a_{21} & a_{22} & \cdots & a_{2j} & \cdots & a_{2n} \\
\vdots & \vdots & \ddots & \vdots & \ddots & \vdots \\
a_{i1} & a_{i2} & \cdots & a_{ij} & \cdots & a_{in} \\
\vdots & \vdots & \ddots & \vdots & \ddots & \vdots \\
a_{m1} & a_{m2} & \cdots & a_{mj} & \cdots & a_{mn} \\
\end{bmatrix}
$$

**Anotações:**

1. **i-ésima linha:** \(\{a_{i1}, a_{i2}, \dots, a_{ij}, \dots, a_{in}\}\)
2. **j-ésima coluna:** \(\begin{bmatrix} a_{1j} \\ a_{2j} \\ \vdots \\ a_{ij} \\ \vdots \\ a_{mj} \end{bmatrix}\)
3. **Elementos:** \(a_{ij}\), onde \(1 \leq i \leq m\) e \(1 \leq j \leq n\).

<!-- MATRIZ (1) pág 9-->

Podemos dizer que $A$ é **$m$ por $n$** (representado por **$m \times n$**). Se $m = n$, dizemos que $A$ é uma **matriz quadrada de ordem $n$** e que os números $a_{11}, a_{22}, \cdots, a_{nn}$ formam a diagonal principal.

Uma matriz $1 \times n$ ou $m \times n$ também é chamada **vetor de dimensão $n$**.