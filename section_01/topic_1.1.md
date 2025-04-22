# Sistemas Lineares

Uma equação do tipo $ax = b$, que expressa a variável $b$ em função da  variável $x$ e da constante $a$, é chamada de **equação linear**. O termo *linear* é utilizado porque o gráfico dessa equação é uma linha reta, conforme ilustrado na Fig. 1.

```{figure} /imgs/graficos_lineares.png
:name: relacao_linear
Relação Linear: Gráficos de b = ax
```


Da mesma forma, a equação

```{math}
:label: eq01
a_1 x_1 + a_2 x_2 + \cdots + a_n x_n = b,
```

que expressa a variável $\color{red}{b}$ em função das variáveis $\color{red}{x_1}$, $\color{red}{x_2}$, $\color{red}{\cdots}$, $\color{red}{x_n}$ e das constantes conhecidas $\color{red}{a_1}$, $\color{red}{a_2}$, $\color{red}{\cdots}$, $\color{red}{a_n}$ é chamada de equação linear. Em diversos cenários, fornecemos $\color{red}{b}$ e as constantes $\color{red}{a_1}$, $\color{red}{a_2}$, $\color{red}{\cdots}$, $\color{red}{a_n}$ e devemos encontrar os números $\color{red}{x_1}$, $\color{red}{x_2}$, $\color{red}{\cdots}$ , $\color{red}{x_n}$ chamados **incógnitas**, que satisfazem a equação.

Uma solução de uma equação linear {math:numref}`eq01` é uma sequência de $\color{red}{n}$ números $\color{red}{s_1}$, $\color{red}{s_2}$, $\color{red}{\cdots}$, $\color{red}{s_n}$ que têm como propriedade satisfazer a expressão {math:numref}`eq01` quando $\color{red}{x_1 = s_1}$, $\color{red}{x_2 = s_2}$, $\color{red}{\cdots}$ , $\color{red}{x_n = s_n}$ são substituídas nessa expressão. Então, $\color{red}{x_1 = 4}$, $\color{red}{x_2 = -1}$ e $\color{red}{x_3 = 2}$ é uma solução para a equação linear:

$$
2x_1 - 3x_2 + 4x_3 = 19,
$$ 

pois, 

$$
2(4)- 3(-1) + 4(2) = 19.
$$

Um sistema de **$\color{red}{m}$ equações lineares a $\color{red}{n}$ incógnitas $\color{red}{x_1}$, $\color{red}{x_2}$, $\color{red}{\cdots}$ , $\color{red}{x_n}$** ou simplesmente um **sistema linear**, é um conjunto de $\color{red}{m}$ equações lineares, cada uma com $\color{red}{n}$ incógnitas.

```{math}
:label: eq02
    \begin{matrix}
        a_{11}x_{1} & + & a_{12}x_{2} & + & \cdots & + & a_{1n}x_{n} & = & b_{1}    \\
        a_{21}x_{1} & + & a_{22}x_{2} & + & \cdots & + & a_{2n}x_{n} & = & b_{2}    \\
        \vdots      &   & \vdots      &   &        &   & \vdots      &   & \vdots   \\
        a_{m1}x_{1} & + & a_{m2}x_{2} & + & \cdots & + & a_{mn}x_{n} & = & b_{m}    \\
    \end{matrix}
```

Uma **solução** de um sistema linear é uma sequência de $\color{red}{n}$ números $\color{red}{s_1}$, $\color{red}{s_2}$, $\color{red}{\cdots}$, $\color{red}{s_n}$ que têm como propriedade o fato de satisfazer cada equação do sistema quando $\color{red}{x_1 = s_1}$, $\color{red}{x_2 = s_2}$, $\color{red}{\cdots}$ , $\color{red}{x_n = s_n}$ são substituídos na expressão. Para resolver um sistema linear, utilizamos uma técnica conhecida como **método da eliminação**.

## Método de Eliminação

O método da eliminação é uma técnica utilizada para resolver sistemas lineares por meio da simplificação gradual do sistema. Seu principal objetivo é eliminar variáveis sucessivamente até que as soluções possam ser facilmente determinadas. Durante o processo, é gerado um novo sistema linear equivalente ao original, ou seja, com exatamente as mesmas soluções. Esse sistema simplificado pode então ser resolvido de forma mais direta.

```{admonition} O método de eliminação pode ser resumido nos seguintes passos:
:class: danger
  1. (Opcional) Trocar a posição de duas equações.  
  2. Multiplicar uma equação por uma constante diferente de zero.
  3. Adicionar um múltiplo de uma equação à outra.
```


:::{include} examples.md
:start-after: <!-- Start Exemple 1.1 -->
:end-before: <!-- End Exemple 1.1 -->
:::

:::{include} examples.md
:start-after: <!-- Start Exemple 1.2 -->
:end-before: <!-- End Exemple 1.2 -->
:::

:::{include} examples.md
:start-after: <!-- Start Exemple 1.3 -->
:end-before: <!-- End Exemple 1.3 -->
:::


```{admonition} Nota
Os exemlos apresentados sugerem que um sistemas linear pode ter **uma única solução**, **nenhuma solução**, ou **infinitas soluções**.
```

01. O sistema tem uma única solução; ou seja, as retas azul e vermelha se cruzam exatamente em um ponto.
02. O sistema não tem solução; ou seja, as relas azul e vermelha não se cruzam.
03. O sistema tem infinitas soluções, ou seja, as retas azul e vermelha são coincidentes.

```{figure} /imgs/grafico_sistemas_lineares.png
:name: relacao_linear
Representação Gráfica de Sistemas Lineares
```