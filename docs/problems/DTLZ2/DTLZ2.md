# **DTLZ2**

## **Definição**

<p style="font-size: 17px;">O problema DTLZ2 possui uma frente ótima de Pareto formada por uma esfera:</p>
$$
\boldsymbol{\textcolor{blue}{f_1^2}(X)} + \boldsymbol{\textcolor{blue}{f_2^2}(X)} +  \underbrace{\boldsymbol{\textcolor{blue}{f_3^2}(X)} + \boldsymbol{....}}_{\text{M > 3} } + \boldsymbol{\textcolor{blue}{f_M^2}(X) = 1} \Longrightarrow \boldsymbol{\sum_{m=1}^M\textcolor{blue}{f_{M}^2} = 1}
$$
<p style="font-size: 17px;">DTLZ2 é definida pelas seguintes variáveis:</p>
<ul style="font-size:17px;">
  <li><strong><i>M</i></strong>: Número de objetivos do problema</li>
  <li><strong><i>N</i></strong>: Número de variáveis de decisão</li>
  <li><strong><i>K</i></strong>: representado por:</li>
</ul>
$$
\boldsymbol{K}\text{ é o valor do vetor } \boldsymbol{\big|X_M\big|} \text{ onde todos } \boldsymbol{X_i} \text{ pertencem a } \boldsymbol{X_M}\text{ }\boldsymbol{(X_i \in X_M)}
$$
<p style="font-size: 17px;">O valor de <strong><i>N</i></strong> pode ser obtido pela equação <strong><i>N = K+M-1</i></strong> substituindo o valor de <strong><i>K</i></strong>. De forma alternativa, pode se definir o valor de <strong><i>K</i></strong> pela equação <strong><i>K = N-M+1</i></strong>, substituindo o valor de <strong><i>N</i></strong>.</p>

## **Exemplo**

### **Para M = 3**
$$
\large \underbrace{f_1}_{\boldsymbol{\textcolor{blue}{f_1}(X)}}, \underbrace{f_2}_{\boldsymbol{\textcolor{blue}{f_{2}}(X)}}, \underbrace{f_3}_{\boldsymbol{\textcolor{blue}{f_M}(X)}}
$$
<p style="font-size: 17px;">Onde <strong><i>f<sub>1</sub> ,f<sub>2</sub> e f<sub>3</sub></i></strong> são as funções objetivo de acordo com o número total de <strong><i>(M = 3)<i></strong>.</p>
<p style="font-size: 17px;">Definir o valor de <strong><i>K<i></strong> assumindo um valor de <strong><i>N = <i></strong>10, pela equação:</p>
<p style="font-size: 17px;"><strong><i>K<i></strong> = 10-3+1 = 8.</p>
<p style="font-size: 17px;"><strong><i>Ou<i></strong></p>
<p style="font-size: 17px;">Definir o valor de <strong><i>N<i></strong> assumindo um valor de <strong><i>K = <i></strong>8, pela equação:</p>
<p style="font-size: 17px;"><strong><i>N<i></strong> = 8+3-1 = 10.</p>
<p style="font-size: 17px;">Para o problema com <strong><i>M<i></strong> = 3, <strong><i>N<i></strong> = 10 e <strong><i>K<i></strong> = 8, temos:</p>
$$
\large x_1, \underbrace{x_2}_{\boldsymbol{X_{M-1}}}, \underbrace{\underbrace{\underbrace{x_3}_{\boldsymbol{X_M}}, x_4, x_5, x_6, x_7, x_8, x_9, x_{10}}_{\boldsymbol{K = \big|X_M\big| = (X_I \in X_M)}}}_{\textcolor{darkred}{\Large \boldsymbol{g(X_M)}}}
$$
<p style="font-size: 17px;">A posição <strong><i>X<sub>M-1</sub></i></strong> e <strong><i>X<sub>M</sub></i></strong> é representada por <strong><i>x<sub>2</sub></i></strong> e <strong><i>x<sub>3</sub></i></strong> respectivamente. O tamanho do vetor <strong><i>| X<sub>M</sub> |</i></strong> é definido pelo valor de <strong><i>K</i></strong> = 8, e se inicia por <strong><i>x<sub>3</sub></i></strong>, percorrendo até o último <strong><i>K = 8</i></strong> váriaveis denotado por <strong><i>x<sub>10</sub></i></strong>.</p>
<p style="font-size: 17px;">A função <span style="color: darkred;"><strong><i>g( X<sub>M</sub> )</i></strong></span> que corresponde as variáveis de decisão dentro do intervalo de <strong><i>| X<sub>M</sub> |</i></strong> ( <strong><i>x<sub>3</sub>  x<sub>4</sub>  x<sub>5</sub>  x<sub>6</sub> x<sub>7</sub>  x<sub>8</sub>  x<sub>9</sub>  x<sub>10</sub></i></strong> ), deve ser <i>minimizada</i> pelos algoritimos evolutivos (<strong><i>MOEAs</i></strong>). Quando o valor desta função atinge <span style="color: darkred;"><strong><i>g = 0</i></strong></span>, encontra-se a frente ótima de Pareto do problema.</p>


### **Para M = 4**
$$
\large \underbrace{f_1}_{\boldsymbol{\textcolor{blue}{f_1}(X)}}, \underbrace{f_2}_{\boldsymbol{\textcolor{blue}{f_2}(X)}}, \underbrace{f_3}_{\boldsymbol{\textcolor{blue}{f_{3}}(X)}}, \underbrace{f_4}_{\boldsymbol{\textcolor{blue}{f_M}(X)}}
$$
<p style="font-size: 17px;">Onde <strong><i>f<sub>1</sub> ,f<sub>2</sub> ,f<sub>3</sub> e f<sub>4</sub></i></strong> são as funções objetivo de acordo com o número total de <strong><i>(M = 4)<i></strong>.</p>
<p style="font-size: 17px;">Definir o valor de <strong><i>K<i></strong> assumindo um valor de <strong><i>N = <i></strong>10, pela equação:</p>
<p style="font-size: 17px;"><strong><i>K<i></strong> = 10-4+1 = 7.</p>
<p style="font-size: 17px;"><strong><i>Ou<i></strong></p>
<p style="font-size: 17px;">Definir o valor de <strong><i>N<i></strong> assumindo um valor de <strong><i>K = <i></strong>7, pela equação:</p>
<p style="font-size: 17px;"><strong><i>N<i></strong> = 7+4-1 = 10.</p>
<p style="font-size: 17px;">Para o problema com <strong><i>M<i></strong> = 4, <strong><i>N<i></strong> = 10 e <strong><i>K<i></strong> = 7, temos:</p>
$$
\large x_1, x_2, \underbrace{x_3}_{\boldsymbol{X_{M-1}}}, \underbrace{\underbrace{\underbrace{x_4}_{\boldsymbol{X_M}}, x_5, x_6, x_7, x_8, x_9, x_{10}}_{\boldsymbol{K = \big|X_M\big| = (X_I \in X_M)}}}_{\textcolor{darkred}{\Large \boldsymbol{g(X_M)}}}
$$
<p style="font-size: 17px;">A posição <strong><i>X<sub>M-1</sub></i></strong> e <strong><i>X<sub>M</sub></i></strong> é representada por <strong><i>x<sub>3</sub></i></strong> e <strong><i>x<sub>4</sub></i></strong> respectivamente. O tamanho do vetor <strong><i>| X<sub>M</sub> |</i></strong> é definido pelo valor de <strong><i>K</i></strong> = 7, e se inicia por <strong><i>x<sub>4</sub></i></strong>, percorrendo até o último <strong><i>K = 7</i></strong> váriaveis denotado por <strong><i>x<sub>10</sub></i></strong>.</p>
<p style="font-size: 17px;">A função <span style="color: darkred;"><strong><i>g( X<sub>M</sub> )</i></strong></span> que corresponde as variáveis de decisão dentro do intervalo de <strong><i>| X<sub>M</sub> |</i></strong> ( <strong><i>x<sub>4</sub>  x<sub>5</sub>  x<sub>6</sub>  x<sub>7</sub> x<sub>8</sub>  x<sub>9</sub>  x<sub>10</sub> )</i></strong>, deve ser <i>minimizada</i> pelos algoritimos evolutivos (<strong><i>MOEAs</i></strong>). Quando o valor desta função atinge <span style="color: darkred;"><strong><i>g = 0</i></strong></span>, encontra-se a frente ótima de Pareto do problema.</p>

## **Funçao g**
<p style="font-size: 17px;">O objetivo da função <span style="color: darkred;"><strong><i>g( X<sub>M</sub> )</i></strong></span> é <strong><i>maximizar a distancia</i></strong> da POF do problema, atraindo os algorítimos evolutivos a POF locais.</p>
<p style="font-size: 17px;">Quando o vetor <strong><i>| X<sub>M</sub> |</i></strong> atinge os valores de <strong><i>| 0.5  0.5 .... 0.5 |</i></strong> a POF do problema é encontrada.</p>
$$
\textcolor{darkred}{\boldsymbol{g(X_M)} = \sum_{X_I\in X_M} (xi-0.5)^2}
$$

## **Funções objetivo**

<p style="font-size: 17px;">Cada função objetivo recebe um valor da função <span style="color: darkred;"><strong><i>g( X<sub>M</sub> )</i></strong></span>. A POF do problema esta diretamente ligada a <span style="color: darkred;"><strong><i>g( X<sub>M</sub> )</i></strong></span>.</p>
$$
\textcolor{blue}{f_1}(X)=(1+\boldsymbol{\textcolor{darkred}{g(X_M)}})\text{ }cos(x_1\pi/2)\text{...} cos(x_{M-2}\pi/2)\text{ } cos(x_{M-1}\pi/2),
$$

$$
\textcolor{blue}{f_2}(X)=(1+\boldsymbol{\textcolor{darkred}{g(X_M)}})\text{ }cos(x_1\pi/2)\text{...} cos(x_{M-2}\pi/2)\text{ } sin(x_{M-1}\pi/2),
$$

$$
\textcolor{blue}{f_3}(X)=(1+\boldsymbol{\textcolor{darkred}{g(X_M)}})\text{ }cos(x_1\pi/2)\text{...} sin(x_{M-2}\pi/2),
$$

$$
\textcolor{blue}{f_3}(X)=(1+\boldsymbol{\textcolor{darkred}{g(X_M)}})\text{ }sin(x_1\pi/2)
$$

## **Métodos**
dtlz2.[POFsamples()](inPOF.md)

dtlz2.[samples()](outPOF.md)


<div style = "text-align: right; margin-top: 2em;">
<button onclick="window.history.back()" style ="font-size:22px;">←</button>
</div>