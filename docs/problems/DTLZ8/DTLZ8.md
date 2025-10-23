# **DTLZ8**

## **Definição**

<p style="font-size: 17px;">O problema DTLZ8 possui uma frente ótima de Pareto formada por uma linha reta, e por um hyperplano linear.</p>
<p style="font-size: 17px;">DTLZ8 é definida pelas seguintes variáveis:</p>
<ul style="font-size:17px;">
  <li><strong><i>M</i></strong>: Número de objetivos do problema</li>
  <li><strong><i>N</i></strong>: Número de variáveis de decisão, representado por: 10<strong><i>M</i></strong></li>
</ul>

## **Camadas**
$$
\large\underbrace{\underbrace{\underbrace{\boldsymbol{x_1} , \boldsymbol{x_2} , \boldsymbol{x_3}}_{\boldsymbol{\textcolor{blue}{f_1}(X)} } , \underbrace{\boldsymbol{x_4} , \boldsymbol{x_5} , \boldsymbol{x_6}}_{\boldsymbol{\textcolor{blue}{f_{M-1}}(X)} }}_{\boldsymbol{\textcolor{darkred}{g_j}(X)}}, \underbrace{\underbrace{\boldsymbol{x_7} , \boldsymbol{x_8} ,\boldsymbol{x_9}}_{\boldsymbol{\textcolor{blue}{f_{M}}(X)} }}_{\boldsymbol{\textcolor{darkred}{g_M}(X)}}}_{\Large\boldsymbol{\big[ \boldsymbol{\textcolor{darkred}{g_j}(X):\boldsymbol{\textcolor{darkred}{g_M}(X)}} \big]\geq 0}}
$$

<p style="font-size: 17px;">O problema pode ser divido em <strong><i>3</i></strong> camadas:</p>
<ul style="font-size:17px;">
  <li>A camada 1 define as funções objetivo</li>
  <li>A camada 2 define a restrição <span style="color: darkred;"><strong><i>g<sub>j</sub> (X)</i></strong></span> responsável pela formação da linha reta que compõe a POF <span style="color: blue;"><strong><i>f<sub>1</sub></i></strong></span> = <span style="color: blue;"><strong><i>f<sub>2</sub></i></strong></span> = ... <span style="color: blue;"><strong><i>f<sub>M-1</sub></i></strong></span>  e a restrição <span style="color: darkred;"><strong><i>g<sub>M</sub> (X)</i></strong></span> que define o hyperplano Linear.</li>
  <li>A camada 3, é o conjunto das restrições, que deve possuir o mesmo número de elementos de <strong><i>M</i></strong> representado por:</li> 
</ul>



### **Camada 1**
<p style="font-size: 17px;">Definição das funções objetivo:</p>
$$
\large\underbrace{\boldsymbol{x_1} , \boldsymbol{x_2} , \boldsymbol{x_3}}_{\boldsymbol{\textcolor{blue}{f_1}(X)} } , \underbrace{\boldsymbol{x_4} , \boldsymbol{x_5} , \boldsymbol{x_6}}_{\boldsymbol{\textcolor{blue}{f_{M-1}}(X)} }, \underbrace{\boldsymbol{x_7} , \boldsymbol{x_8} ,\boldsymbol{x_9}}_{\boldsymbol{\textcolor{blue}{f_{M}}(X)} }
$$
<ul style="font-size:17px;">
  <li><span style="color: blue;"><strong><i>f<sub>j</sub></i></strong></span> <strong><i>(X)</i></strong> </li>
</ul>
$$
\boldsymbol{\textcolor{blue}{f_{j}}(X)}=   \large   \frac{1}{\big[\frac{n}{M}\big]}  \sum\nolimits_{\big[(\text{ j - 1 })\frac{n}{M}\big]}^{\big[j\frac{n}{M}\big]} \boldsymbol{x_i},
$$


### **Camada 2**
<p style="font-size: 17px;">Definição das Restrições:</p>
$$
\underbrace{\boldsymbol{\textcolor{blue}{f_{1}}(X)} \boldsymbol{\text{ ... }} \boldsymbol{\textcolor{blue}{f_{M-1}}(X)}}_{\Large\boldsymbol{\textcolor{darkred}{g_j}(X)} }, \underbrace{\boldsymbol{\textcolor{blue}{f_{M}}(X)}}_{\Large\boldsymbol{\textcolor{darkred}{g_M}(X)}}
$$
<ul style="font-size:17px;">
  <li><span style="color: darkred;"><strong><i>g<sub>j</sub> (X)</i></strong></span> </li>
</ul>
$$
\boldsymbol{\textcolor{darkred}{g_{j}}(X)} = \boldsymbol{\textcolor{blue}{f_M}(X)} + 4\boldsymbol{\textcolor{blue}{f_j}(X)} - 1 \geq 0
$$
<ul style="font-size:17px;">
  <li><span style="color: darkred;"><strong><i>g<sub>M</sub> (X)</i></strong></span> </li>
</ul>
$$
\boldsymbol{\textcolor{darkred}{g_{M}}(X)} = 2 \boldsymbol{\textcolor{blue}{f_M}(X)} + {\large \min\limits_{\substack{\scriptstyle i,j=1\\ \scriptstyle i\#j}}^{ M-1 }} \text{ } \big[\boldsymbol{\textcolor{blue}{f_i}(X)}+\boldsymbol{\textcolor{blue}{f_j}(X)}\big] \geq 0
$$


### **Camada 3**
<p style="font-size: 17px;">Junção do conjunto de restrições:</p>
<ul style="font-size:17px;">
  <li><span style="color: darkred;"><strong><i>g<sub>j</sub> (X)</i></strong></span> e <span style="color: darkred;"><strong><i>g<sub>M</sub> (X)</i></strong></span></li>
</ul>


$$
\underbrace{\boldsymbol{\textcolor{darkred}{g_j}(X)\big[\boldsymbol{\textcolor{blue}{f_{1}}(X)} \boldsymbol{\text{ ... }} \boldsymbol{\textcolor{blue}{f_{M-1}}(X)}\big] \text{ , } } \boldsymbol{\textcolor{darkred}{g_M}(X)\big[\boldsymbol{\textcolor{blue}{f_{M}}(X)}\big]}}_{\Large\boldsymbol{ \big[ \boldsymbol{\textcolor{darkred}{g_j}(X):\boldsymbol{\textcolor{darkred}{g_M}(X)}} \big]\geq 0}}
$$

## **Exemplo**
<p style="font-size: 17px;">Problema definido com:</p>
<ul style="font-size:17px;">
  <li><strong><i>M = 4</i></strong> </li>
  <li><strong><i>N = 3M = 12</i></strong> </li>
</ul>


<ul style="font-size:17px;">
  <li><span style="color: blue;"><strong><i>f<sub>j</sub></i></strong></span></li>
</ul>
$$
\boldsymbol{\textcolor{blue}{f_{1}}(X)}=   \large   \frac{1}{\big[\frac{12}{4}\big]}  \sum\nolimits_{\big[(\text{ 1 - 1 })\frac{12}{4}\big]}^{\big[1\frac{12}{4}\big]} =\normalsize 0.35 * \underbrace{(x1+x2+x3)}_{\large  x\big[1:3\big]}
$$

$$
\boldsymbol{\textcolor{blue}{f_{2}}(X)}=   \large   \frac{1}{\big[\frac{12}{4}\big]}  \sum\nolimits_{\big[(\text{ 2 - 1 })\frac{12}{4}\big]}^{\big[2\frac{12}{4}\big]} =\normalsize 0.35 * \underbrace{(x4+x5+x6)}_{\large   x\big[4:6\big]}
$$

$$
\boldsymbol{\textcolor{blue}{f_{(3)M-1}}(X)}=   \large   \frac{1}{\big[\frac{12}{4}\big]}  \sum\nolimits_{\big[(\text{ 3 - 1 })\frac{12}{4}\big]}^{\big[3\frac{12}{4}\big]} =\normalsize 0.35 * \underbrace{(x7+x8+x9)}_{\large   x\big[7:9\big]}
$$

$$
\boldsymbol{\textcolor{blue}{f_{(4)M}}(X)}=   \large   \frac{1}{\big[\frac{12}{4}\big]}  \sum\nolimits_{\big[(\text{ 4 - 1 })\frac{12}{4}\big]}^{\big[4\frac{12}{4}\big]} \normalsize = 0.35 * \underbrace{(x10+x11+x12)}_{\large x\big[10:12\big]}
$$


<ul style="font-size:17px;">
  <li><span style="color: darkred;"><strong><i>g<sub>j</sub> (X)</i></strong></span></li>
</ul>
<p style="font-size: 17px;">Compreende o intervalo: <span style="color: blue;"><strong><i>f<sub>1</sub>  f<sub>2</sub>  f<sub>(3)M-1</sub></i></strong></span></p>
$$
\boldsymbol{\textcolor{darkred}{g_{1}}(X)} = \boldsymbol{\textcolor{blue}{f_{(4)}M}(X)} + 4\boldsymbol{\textcolor{blue}{f_1}(X)} - 1 \geq 0
$$

$$
\boldsymbol{\textcolor{darkred}{g_{2}}(X)} = \boldsymbol{\textcolor{blue}{f_{(4)}M}(X)} + 4\boldsymbol{\textcolor{blue}{f_2}(X)} - 1 \geq 0
$$

$$
\boldsymbol{\textcolor{darkred}{g_{3}}(X)} = \boldsymbol{\textcolor{blue}{f_{(4)}M}(X)} + 4\boldsymbol{\textcolor{blue}{f_3}(X)} - 1 \geq 0
$$

<ul style="font-size:17px;">
  <li><span style="color: darkred;"><strong><i>g<sub>M</sub> (X)</i></strong></span></li>
</ul>
$$
{\large \min\limits_{\substack{\scriptstyle i,j=1\\ \scriptstyle i\#j}}^{ M-1 }} \text{ } \big[\boldsymbol{\textcolor{blue}{f_i}(X)}+\boldsymbol{\textcolor{blue}{f_j}(X)}\big] 
$$
<p style="font-size: 17px;">Calcula a menor soma entre as combinações dos objetivos <span style="color: blue;"><strong><i> f<sub>1  </sub>f<sub>2  </sub>f<sub>(3)M-1</sub></i></strong></span>, desde que não sejam pares de objetivos iguais: <span style="color: blue;"><strong><i>[ ( f<sub>1</sub> + f<sub>2</sub> ), ( f<sub>1</sub> + f<sub>3</sub> ) , ( f<sub>2</sub> + f<sub>3</sub> ) ] </i></strong></span></p>. 
<p style="font-size: 17px;">Supondo que a menor soma é <span style="color: blue;"><strong><i>( f<sub>2</sub> + f<sub>3</sub> )</strong></span></p>
$$
\boldsymbol{\textcolor{darkred}{g_{(4)M}}(X)} = 2 \boldsymbol{\textcolor{blue}{f_{(4)M}}(X)} + \text{ } (\boldsymbol{\textcolor{blue}{f_2}(X)}+\boldsymbol{\textcolor{blue}{f_3}(X)}) \geq 0
$$

<ul style="font-size:17px;">
  <li><span style="color: darkred;"><strong><i>Restrições</strong></span>:<span style="color: darkred;"></li>
</ul>

$$
\boldsymbol{\underbrace{\underbrace{\textcolor{blue}{f_1}(x)}_{\Large\textcolor{darkred}{g_1}(x)} \text{  }\underbrace{\textcolor{blue}{f_2}(x)}_{\Large\textcolor{darkred}{g_2}(x)}\text{  } \underbrace{\textcolor{blue}{f_{3}}(x)}_{\Large\textcolor{darkred}{g_{3}}(x)}}_{\Large\textcolor{darkred}{g_j}} \text{  } \underbrace{\underbrace{\textcolor{blue}{f_{4}}(x)}_{\Large\textcolor{darkred}{g_{4}}(x)}}_{\Large\textcolor{darkred}{g_M}}}
$$
<p style="font-size: 17px;">O número de funções objetivo <span style="color: blue;"><strong><i>M = 4</i></strong></span> é o mesmo número de restrições <span style="color: darkred;"><strong><i>g = 4</i></strong></span>. Para as 4 funções objetivo serem válidas, a condição <span style="color: darkred;"><strong><i>g<sub>j</sub> (x) : g<sub>M</sub> (x) ≥ 0</i></strong></span> deve ser satisfeita</p>











## **Métodos**
dtlz8.[POFsamples()](inPOF.md)

dtlz8.[samples()](outPOF.md)


<div style = "text-align: right; margin-top: 2em;">
<button onclick="window.history.back()" style ="font-size:22px;">←</button>
</div>