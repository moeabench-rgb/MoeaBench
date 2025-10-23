# Amostras dominadas 

## **Método**

<p style="font-size: 17px;">O método <strong><i>dtlz2.samples()</i></strong> não altera o vetor <strong><i>| X<sub>M</sub> |</i></strong>. A finalidade é preservar a <i>maximização</i> da função <span style="color: darkred;"><strong><i>g( X<sub>M</sub> )</i></strong></span>, gerando mínimos locais sobre a verdadeira frente ótima de Pareto. O objetivo desta função é dificultar a resolução do problema pelos algorítimos evolutivos( <strong><i>MOEAs</i></strong> ).</p>

## **Configuração**

<p style="font-size: 17px;">O método poasui a seguinte configuração <strong><i>padrão</i></strong>:</p>
<ul style="font-size:17px;">
  <li><strong><i>M</i></strong>( objetivos do problema ) = 3</li>
  <li><strong><i>N</i></strong>( variáveis de decisão ) = 10</li>
  <li><strong><i>K</i></strong>( valor para o tamanho do vetor <strong><i>| X<sub>M</sub> |</i></strong> ) = 8</li>
  <li><strong><i>P</i></strong>( númetos de pontos / soluções do problema ) = 700</li>
</ul>
<p style="font-size: 17px;">O método aceita qualquer configuração de valores para as variáveis do problema, incluindo qualquer número para <strong><i>M</i></strong>.</p> 

## **Arquivo**

O método gera um arquivo com extensão <strong><i>.XLSX</i></strong> que pode ser utilizado pelas ferramentas de análise de dados do <strong><i>Evobench</i></strong></p>

## **Figura**

![Engine](DTLZ2outPOF.png)

<p style="font-size: 17px;">Figura gerada por uma das ferramentas de plotagem de gráficos do <strong><i>Evobench</i></strong>.</p>

## **Amostragem**

<p style="font-size: 17px;">Os valores das variáveis de decisão, são gerados de forma randômica respeitando o seguinte critério: <strong><i>0 ≤ x<sub>i</sub> ≤ 1</i></strong> para <strong><i>i = 1,2 ... N</i></strong>.</p>

<div style = "text-align: right; margin-top: 2em;">
<button onclick="window.history.back()" style ="font-size:22px;">←</button>
</div>

