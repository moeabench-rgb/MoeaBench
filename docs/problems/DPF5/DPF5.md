# **DPF5**

## **Definição**

<p style="font-size: 17px;">O problema DPF5 possui uma frente ótima de Pareto formada por:</p>


$$
\boldsymbol{\textcolor{blue}{f_1^2}(X)} + \boldsymbol{\textcolor{blue}{f_2^2}(X)} +  \underbrace{\boldsymbol{\textcolor{blue}{f_3^2}(X)} + \boldsymbol{....}}_{\text{M > 3} } + \boldsymbol{\textcolor{blue}{f_M^2}(X) = 1} \Longrightarrow \boldsymbol{\sum_{m=1}^M\textcolor{blue}{f_{m}^2} = 1}
$$
<p style="font-size: 17px;">DPF5 é definida pelas seguintes variáveis:</p>
<ul style="font-size:17px;">
  <li><strong><i>M</i></strong>: Número de objetivos do problema</li>
  <li><strong><i>N</i></strong>: Número de variáveis de decisão</li>
  <li><strong><i>D</i></strong>: Número de objetivos essenciais</li>
  <li><strong><i>K</i></strong>: representado por:</li>
</ul>
$$
\boldsymbol{K}\text{ é o valor do vetor } \boldsymbol{\big|X^{\large r}\big|} \text{ onde todos } \boldsymbol{X_i} \text{ }\boldsymbol{(X_m \in X_n)}
$$

<p style="font-size: 17px;">O valor de <strong><i>N</i></strong> pode ser obtido pela equação <strong><i>N = D+K-1</i></strong>.</p>


## **Disposição**

<p style="font-size: 17px;">O problema é dividido em 2 partes:</p>

<ul style="font-size:17px;">
  <li><strong><i>M-D</i></strong>: Onde estão localizados os objetivos redundantes, que podem variar de acordo com o tamanho de M e de D. Também pode sofrer alterações nos objetivos de acordo com o valor da variavel de decisão <strong><i>x<sub>1</sub></i></strong></li>
  <li><strong><i>M-D+1</i></strong>: Onde estão localizados os objetivos essenciais do problema, que possui o tamanho de <strong><i>D</i></strong> objetivos.</li>
</ul>

### **m - d**

<ul style="font-size:17px;">
  <li><strong><i>M-D</i></strong>: Objetivos redundantes</li>
</ul>


#### **Combinações**

##### **m - d = 1**
$$
\begin{array}{l}  \boldsymbol{\textcolor{blue}{f_1}} = \left\{ \begin{array}{l} \boldsymbol{x_1 > \frac{1}{3} \rightarrow \textcolor{blue}{\gamma_1}} \\ ou \\ \boldsymbol{x_1 < \frac{1}{3} \rightarrow \textcolor{blue}{\beta_1}} \end{array}\right.          \end{array}
$$


##### **m - d = 2**


$$
\begin{array}{l}  \boldsymbol{\textcolor{blue}{f_1}} = \left\{ \begin{array}{l} \boldsymbol{x_1 > \frac{1}{3} \rightarrow \textcolor{blue}{\gamma_1}} \\ ou \\ \boldsymbol{x_1 < \frac{1}{3} \rightarrow \textcolor{blue}{\beta_1}} \end{array}\right.{\large\boldsymbol{,}}&    \boldsymbol{\textcolor{darkgreen}{f_2}} = \left\{ \begin{array}{l} \boldsymbol{x_1 > \frac{1}{3} \rightarrow \textcolor{darkgreen}{\gamma_2}} \\ ou \\ \boldsymbol{x_1 < \frac{1}{3} \rightarrow \textcolor{darkgreen}{\beta_2}} \end{array}\right.  \end{array}
$$

##### **m - d > n**

$$
\begin{array}{l}  \boldsymbol{\textcolor{blue}{f_1}} = \left\{ \begin{array}{l} \boldsymbol{x_1 > \frac{1}{3} \rightarrow \textcolor{blue}{\gamma_1}} \\ ou \\ \boldsymbol{x_1 < \frac{1}{3} \rightarrow \textcolor{blue}{\beta_1}} \end{array}\right. {\large\boldsymbol{,}}  &    \boldsymbol{\textcolor{darkgreen}{f_2}} = \left\{ \begin{array}{l} \boldsymbol{x_1 > \frac{1}{3} \rightarrow \textcolor{darkgreen}{\gamma_2}} \\ ou \\ \boldsymbol{x_1 < \frac{1}{3} \rightarrow \textcolor{darkgreen}{\beta_2}} \end{array}\right.&\boldsymbol{\textcolor{darkgreen}{\begin{array}{l}\textbf{..}\end{array}}}{\large\boldsymbol{,}}&  \boldsymbol{\textcolor{darkgreen}{f_{m-d}}} = \left\{ \begin{array}{l} \boldsymbol{x_1 > \frac{1}{3} \rightarrow \textcolor{darkgreen}{\gamma_2}} \\ ou \\ \boldsymbol{x_1 < \frac{1}{3} \rightarrow \textcolor{darkgreen}{\beta_2}} \end{array}\right.      \end{array}
$$

### **m - d + 1**

<ul style="font-size:17px;">
  <li><strong><i>M-D</i></strong>: Objetivos essenciais</li>
</ul>


#### **Combinações**

##### **d = 2**


$$
\begin{array}{l}  \boldsymbol{\textcolor{blue}{f_{m-d+1}}} = \left\{ \begin{array}{l} \boldsymbol{x_1 > \frac{1}{3} \rightarrow \textcolor{blue}{\gamma_1}} \\ ou \\ \boldsymbol{x_1 < \frac{1}{3} \rightarrow \textcolor{blue}{\beta_{m-d+1}}} \end{array}\right.{\large\boldsymbol{,}}&  \boldsymbol{\textcolor{blue}{f_{m}}} \begin{array}{l} = \boldsymbol{\textcolor{blue}{\gamma_d}}              \end{array}          \end{array}
$$

##### **d = 3**


$$
\begin{array}{l}  \boldsymbol{\textcolor{blue}{f_{m-d+1}}} = \left\{ \begin{array}{l} \boldsymbol{x_1 > \frac{1}{3} \rightarrow \textcolor{blue}{\gamma_1}} \\ ou \\ \boldsymbol{x_1 < \frac{1}{3} \rightarrow \textcolor{blue}{\beta_{m-d+1}}} \end{array}\right.{\large\boldsymbol{,}}&    \boldsymbol{\textcolor{darkgreen}{f_{m-1}}} \begin{array}{l} = \boldsymbol{\textcolor{darkgreen}{\gamma_{d-1}}} \end{array}{\large\boldsymbol{,}}& \boldsymbol{\textcolor{blue}{f_{m}}}            \begin{array}{l} = \boldsymbol{\textcolor{blue}{\gamma_d}}                          \end{array}    \end{array}
$$

##### **d = 4**

$$
\begin{array}{l}  \boldsymbol{\textcolor{blue}{f_{m-d+1}}} = \left\{ \begin{array}{l} \boldsymbol{x_1 > \frac{1}{3} \rightarrow \textcolor{blue}{\gamma_1}} \\ ou \\ \boldsymbol{x_1 < \frac{1}{3} \rightarrow \textcolor{blue}{\beta_{m-d+1}}} \end{array}                                           \right.{\large\boldsymbol{,}}&    \boldsymbol{\textcolor{darkgreen}{f_{m-d+2}}} \begin{array}{l} = \boldsymbol{\textcolor{darkgreen}{\gamma_2}}              \end{array}{\large\boldsymbol{,}}& \boldsymbol{\textcolor{darkgreen}{f_{m-1}}} \begin{array}{l} = \boldsymbol{\textcolor{darkgreen}{\gamma_{d-1}}} \end{array}{\large\boldsymbol{,}}& \boldsymbol{\textcolor{blue}{f_{m}}} \begin{array}{l} = \boldsymbol{\textcolor{blue}{\gamma_d}}              \end{array}            \end{array}
$$

##### **d = n**


$$
\begin{array}{l}  \boldsymbol{\textcolor{blue}{f_{m-d+1}}} = \left\{ \begin{array}{l} \boldsymbol{x_1 > \frac{1}{3} \rightarrow \textcolor{blue}{\gamma_1}} \\ ou \\ \boldsymbol{x_1 < \frac{1}{3} \rightarrow \textcolor{blue}{\beta_{m-d+1}}} \end{array}\right.{\large\boldsymbol{,}}&    \boldsymbol{\textcolor{darkgreen}{f_{m-d+2}}} \begin{array}{l} = \boldsymbol{\textcolor{darkgreen}{\gamma_2}}              \end{array}&  \boldsymbol{\textcolor{darkgreen}{\begin{array}{l}\textbf{..}\end{array}}}{\large\boldsymbol{,}}& \boldsymbol{\textcolor{darkgreen}{f_{m-1}}} \begin{array}{l} = \boldsymbol{\textcolor{darkgreen}{\gamma_{d-1}}}\end{array}{\large\boldsymbol{,}}&                           \boldsymbol{\textcolor{blue}{f_{m}}} \begin{array}{l} = \boldsymbol{\textcolor{blue}{\gamma_d}}              \end{array}              \end{array}
$$

## **Redundância**

<p style="font-size: 17px;">Problemas de Benchmark de teste para otimização multiobjeto, possuem normalmente uma frente de pareto definida por M-1 dimensões, com todos seus objetivos conflitantes entre si, ou seja independentes um dos outros. A presença de objetivos redundantes, torna a dimensão da frente ótima de Pareto  degenerada, ou seja menor que M-1.</p>

<ul style="font-size:17px;">
  <li><strong><i>M = 10: </i></strong>objetivos do problema</li>
  <li><strong><i>D = 5: </i></strong>objetivos essenciais</li>
  <li><strong><i>M-D = 5: </i></strong>objetivos redundantes</li>
</ul>
  
### **X<sub>1</sub> > 1/3**

<p style="font-size: 17px;">O número de objetivos redundantes aumentam de acordo com o valor de <strong><i>m - d</i></strong> e com a variável de decisão <strong><i>X<sub>1</sub> > &frac13; </i></strong></p>

$$
\boldsymbol{\underbrace{\underbrace{\textcolor{red}{\;\underbrace{\overbrace{\gamma_1}^{f_1}}_{\textbf{redundante}}\;\;\underbrace{\overbrace{\gamma_2}^{f_2}\;\;\overbrace{\gamma_2}^{f_3}\;\;\overbrace{\gamma_2}^{f_4}\;\;\overbrace{\gamma_2}^{f_5}}_{\textbf{redundante}}}}_{\overline{m-d}}\;\;\underbrace{\;\textcolor{blue}{\underbrace{\textcolor{blue}{\overbrace{\gamma_1}^{f_6}}\;\;\textcolor{blue}{\overbrace{\gamma_2}^{f_7}}}_{\textbf{conflitante}}}\;\;\textcolor{red}{\underbrace{\overbrace{\gamma_2}^{f_8}}_{\textbf{redundante}}}\;\;\textcolor{blue}{    \underbrace{ \overbrace{\gamma_{d-1}}^{f_9}}_{\textbf{conflitante}\;}}}_{\overline{d-1}}}   _{\overline{m-1}}\;\;\underbrace{\underbrace{\textcolor{blue}{\underbrace{\overbrace{\gamma_d}^{f_{10}}}_{\;\textbf{conflitante}}\;}}_{\overline{d}}}_{\overline{m}}}
$$


<p style="font-size: 17px;">Acima, na divisão <strong><i>m - d</i></strong>, existem dois segmentos <span style="color: darkred;"><strong><i>( &gamma;<sub>1 , </sub>&gamma;<sub>2</sub> )</i></strong></span>  que estão redundantes dentro do problema, totalizando <strong><i>5 objetivos</i></strong>. Na divisão <strong><i>d</i></strong>, no segmento <strong><i>d - 1</i></strong> estão localizados os objetivos essenciais. Neste segmento, também existe um objetivo redundante <strong><i>&gamma;<sub>2</sub></i></strong>, em função do valor de <strong><i>d > 4</i></strong> . Na divisão <strong><i>m - 1</i></strong> que engloba as divisões <strong><i>m - d</i></strong> e  <strong><i>d</i></strong> os segmentos <span style="color: blue;"><strong><i>( &gamma;<sub>1 , </sub>&gamma;<sub>2</sub> , </sub>&gamma;<sub>d-1</sub> )</i></strong></span> são conflitantes entre si, toalizando <strong><i>3 objetivos</i></strong>.</p>.

### **X<sub>1</sub> < 1/3**

<p style="font-size: 17px;">O número de objetivos redundantes também aumentam de acordo com o valor de <strong><i>m - d</i></strong>, mas o número de objetivos redudantes pode ser menor em função da variável de decisão <strong><i>X<sub>1</sub> < &frac13; </i></strong>.</p>

$$
\boldsymbol{\underbrace{\underbrace{\textcolor{blue}{\;\underbrace{\overbrace{\beta_1}^{f_1}\;\overbrace{\beta_2}^{f_2}}_{\textbf{conflitante}}      \;\;\textcolor{red}{\underbrace{\overbrace{\beta_2}^{f_3}\;\;\overbrace{\beta_2}^{f_4}\;\;\overbrace{\beta_2}^{f_5}}_{\textbf{redundante}}}}}_{\overline{m-d}}\;\;\underbrace{\;\textcolor{blue}{\underbrace{\textcolor{blue}{\overbrace{\beta_{m-d+1}}^{f_6}}\;\;\textcolor{blue}{\overbrace{\gamma_2}^{f_7}}}_{\textbf{conflitante}}}\;\;\textcolor{red}{\underbrace{\overbrace{\gamma_2}^{f_8}}_{\textbf{redundante}}}\;\;\textcolor{blue}{    \underbrace{ \overbrace{\gamma_{d-1}}^{f_9}}_{\textbf{conflitante}\;}}}_{\overline{d-1}}}   _{\overline{m-1}}\;\;\underbrace{\underbrace{\textcolor{blue}{\underbrace{\overbrace{\gamma_d}^{f_{10}}}_{\;\textbf{conflitante}\; }}}_{\overline{d}}}_{\overline{m}}}
$$

<p style="font-size: 17px;">Acima, na divisão <strong><i>m - d</i></strong>, existe um segmentos <span style="color: darkred;"><strong><i>( &beta;<sub>2</i> )</strong></span>  que estão redundantes dentro do problema, totalizando <strong><i>3 objetivos</i></strong>. Na divisão <strong><i>d</i></strong>, no segmento <strong><i>d - 1</i></strong> estão localizados os objetivos essenciais. Neste segmento, também existe um objetivo redundante <strong><i>&beta;<sub>2</sub></i></strong>, em função do valor de <strong><i>d > 4</i></strong>. Na divisão <strong><i>m - 1</i></strong> que engloba as divisões <strong><i>m - d</i></strong> e  <strong><i>d</i></strong> os segmentos <span style="color: blue;"><strong><i>( &beta;<sub>1</sub> , &beta;<sub>2</sub> , &beta;<sub>m - d +1</sub> , &gamma;<sub>2</sub> , </sub>&gamma;<sub>d-1</sub> )</i></strong></span> são conflitantes entre si, toalizando <strong><i>5 objetivos</i></strong>.</p>.

## **Funçao g**

$$
{ \underbrace{x1}_{\large \boldsymbol{m-2}} , \underbrace{x2}_{\underbrace{ \large \boldsymbol{m-1}}_{ \Large \boldsymbol{d-2}}  } , \underbrace{x3}_{\underbrace{ \large \boldsymbol{M}}_{ \Large \boldsymbol{d-1}}} ,  \underbrace{\underbrace{ \underbrace{x4}_{\underbrace{\underbrace{\large \boldsymbol{m+1}}_{\Large \boldsymbol{d}} }_{{ \Large \boldsymbol{X_m}}}} , x5  ,x6  , x7 , x8  ,x9 , x10 , x11 , x12 , \underbrace{x13}_{\large \boldsymbol{X_n}}}_{\large \boldsymbol{X^{\huge r}}}}_{\textcolor{darkred}{\Large \boldsymbol{g(X^{\huge r})}}}}
$$


<p style="font-size: 17px;">A posição <strong><i>X<sub>M</sub></i></strong> e <strong><i>X<sub>M+1</sub></i></strong> é representada por <strong><i>x<sub>3</sub></i></strong> e <strong><i>x<sub>4</sub></i></strong> respectivamente. O tamanho do vetor <strong><i>| X<sup>r</sup> |</i></strong> é definido pelo valor de <strong><i>K</i></strong> = 10, e corresponde ao intervalo de <strong><i>x<sub>4</sub></i></strong> até <strong><i>X<sub>n</sub></i></strong> váriaveis denotado por <strong><i>x<sub>13</sub></i></strong>.</p>
<p style="font-size: 17px;">A função <span style="color: darkred;"><strong><i>g( X<sup>r</sup> )</i></strong></span> que corresponde as variáveis de decisão dentro do intervalo de <strong><i> X<sup>r</sup> = </i></strong> ( <strong><i>x<sub>4</sub>  x<sub>5</sub>  x<sub>6</sub>  x<sub>7</sub> x<sub>8</sub>  x<sub>9</sub>  x<sub>10</sub>  x<sub>11</sub>  x<sub>12</sub>  x<sub>13</sub></i></strong> ), deve ser <i>minimizada</i> pelos algoritimos evolutivos (<strong><i>MOEAs</i></strong>). Quando o valor desta função atinge <span style="color: darkred;"><strong><i>g = 0</i></strong></span>, pode-se econtrar a  frente ótima de Pareto do problema em paralelo a habilidade dos <strong><i>MOEAs</i></strong> em ignorar os objetivos redundantes da POF do problema, que é degenerada. A definição da forma da POF é menor que o segmento M-1</p>


<p style="font-size: 17px;">O objetivo da função <span style="color: darkred;"><strong><i>g( X<sup>r</sup> )</i></strong></span> é <strong><i>maximizar a distancia</i></strong> da POF do problema, atraindo os algorítimos evolutivos a POF locais. Além disso o problema pode conter varios objetivos redundantes, dificultando ainda mais a busca pela frente ótima de Pareto</p>
<p style="font-size: 17px;">Quando o vetor <strong><i>| X<sub>M</sub> |</i></strong> atinge os valores de <strong><i>| 0.5  0.5 .... 0.5 |</i></strong> a POF pode ser encontrada, em paralelo com a eficácia dos <strong><i>MOEAs</i></strong> em ignorar objetivos redundantes e buscar apenas por objetivos essenciais, que são conflitantes dentro do problema .</p>
$$
\boldsymbol{\textcolor{darkred}{g(X^{\large r}) = (x_m-x_i)^2 + \boldsymbol{\displaystyle\sum^{\boldsymbol{n}}_{\boldsymbol{i = m + 1}}} \boldsymbol{(x_i-0.5)^2}}};
$$





## **Funções objetivo**

<p style="font-size: 17px;">Algumas das variáveis de decisão das função objetivo são separáveis e outras dependentes. Cada função objetivo recebe um valor da função <span style="color: darkred;"><strong><i>g( X<sup>r</sup> )</i></strong></span>. A POF do problema esta ligada a minimização de <span style="color: darkred;"><strong><i>g( X<sub>r</sub> )</i></strong></span>, e na busca por objetivos que sejam essenciais ap problema.</p>

$$
 \beta_1(X) = \cos(\theta_1). . . \cos(\theta_{m-2})\cos(\theta_{m-1})(1+\boldsymbol{\textcolor{darkred}{g(X^{\large r})}});
$$

$$
 \beta_2(X) = \cos(\theta_1). . . \cos(\theta_{m-2})\sin(\theta_{m-1})(1+\boldsymbol{\textcolor{darkred}{g(X^{\large r})}});
$$

$$
 \beta_{m-d+1}(X) = \cos(\theta_1). . . \cos(\theta_{d-1})\sin(\theta_{d})(1+\boldsymbol{\textcolor{darkred}{g(X^{\large r})}});
$$

$$
 \gamma_1(X) = \sqrt{\frac{1}{m-d+1}} \cos(\theta_1). . . \cos(\theta_{d-1})(1+\boldsymbol{\textcolor{darkred}{g(X^{\large r})}});
$$

$$
 \gamma_2(X) =  \cos(\theta_1). . . \cos(\theta_{d-2}) \sin(\theta_{d-1})(1+\boldsymbol{\textcolor{darkred}{g(X^{\large r})}});
$$

$$
 \gamma_{d-1}(X) =  \cos(\theta_1)\sin(\theta_2) (1+\boldsymbol{\textcolor{darkred}{g(X^{\large r})}});
$$

$$
\gamma_d(X) =  \sin(\theta_1) (1+\boldsymbol{\textcolor{darkred}{g(X^{\large r})}});
$$

$$
\theta_j = \frac{\pi}{2} x_j \;\;onde\;\; j \in \{1...,m-1\},
$$




## **Métodos**


dpf5.[POFsamples()](inPOF.md)

dpf5.[samples()](outPOF.md)

<div style = "text-align: right; margin-top: 2em;">
<button onclick="window.history.back()" style ="font-size:22px;">←</button>
</div>