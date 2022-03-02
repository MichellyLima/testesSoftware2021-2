<div align=center>
  <img src="brasaooficialcolorido.png">
</div>

#### <p style="text-align: center;">Universidade Federal de Goiás</p>
#### <p style="text-align: center;">Instituto de Informática</p>
#### <p style="text-align: center;">Bacharelado em Engenharia de Software</p>
#### <p style="text-align: center;">Teste de Software - 2021/2</p>
#### <p style="text-align: center;">Gilmar Ferreira Arantes</p>
####  <p style="text-align: center;"> Prova P1 - 16/02/2022</p>

Matrícula: 201802780
Nome: Michelly Silva Lima

<p><font color=green>Nota: 9,3.</font></p>

1. Quanto ao objetivo do Teste de Software, responda as duas questões seguintes:
   1. (**0,5 ponto**) Qual o objetivo primário da atividade de teste de software?
   R: O objetivo do teste de software é revelar a presença de defeitos no software, garantindo que o mesmo se comporta como esperado e também garantindo a qualidade do produto testado. <font color=green>Certo.</font><br/><br/>

   2. (**0,5 ponto**) O que acontece, quando não se atinge este objetivo primário?
   R: Caso a presença de defeitos não seja detectada pelos testes, a abordagem ou método de testagem deve ser alterada, pois o atual não foi capaz de detectar os defeitos existentes. Nenhum software está livre de defeitos, portanto, deve-se testar exaustivamente até que o objetivo primário se cumpra. <font color=red>Errado.</font><br/><br/>

2. (**1,0 ponto**) Explique o que é o teste exaustivo e porque sua execução não é possível.
R: O teste exaustivo é a técnica de se aplicar todas as possibilidades de entradas possíveis em um software para garantir que este se comporta como esperado. Sua execução se torna impossível por fatores de prazo e custo de testes. Geralmente, não temos tempo hábil e esforço suficientes para executá-lo e mesmo que tivessemos, o custo de Teste seria tamanho que tornaria o seu custo inviável. <font color=green>Certo.</font><br/><br/>

3. (**1,0 ponto**) Cite pelo menos duas limitações da Técnica de Teste Funcional e duas da Técnica de Teste Estrutural.
R: A técnica de Teste Funcional, por levar em conta apenas os requisitos funcionais do software, possui as limitações de não ser possível testar os detalhes da implementação como tempo de execução e complexidade e, além disso, a especificação dos requisitos geralmente é informal e, dessa forma, a cobertura total dos casos de teste cujos dados foram obtidos desta especificação  também é informal. <br/> Já a técnica de Teste Estrutural, que tem como objetivo avaliar a estrutura interna do software, possui as limitações de não conseguir avaliar funções omitidas, erros de interface ou erros de comportamento. <font color=green>Certo.</font><br/><br/>

4. (**1,0 ponto**) Descreva pelo menos um dos quatro níveis de teste constantes da literatura especializada.
R: Os Testes de Unidate (Unit Testing) é o 4º nível de teste, em que se é verificado os elementos do software a nível de código. Uma unidade é a menor parte testável de um software e, portanto, esse teste é aplicado aos componentes da implementação, validando suas entradas e saídas, assim como se os fluxos de controle e de dados que foram desenvolvidos estão sendo considerados e se funcionam conforme o esperado. <font color=green>Certo.</font><br/><br/>

5. (**1.0 ponto**)Descreva qual o propósito do critério de teste funcional Particionamento por Classes de Equivalência.
R: O Particionamento por Equivalência possui o objetivo de reduzir o número de casos de teste, mas ainda assim, garantindo uma boa cobertura do código do software em teste. Para isso, divide-se o domínio dos valores de entrada em classes de equivalência válidas e inválidas e, após isso, seleciona-se o menor número possível de casos de teste, considerando que um elemento que pertença à classe definida represente toda a classe de equivalência. <font color=green>Certo.</font> <br/><br/>

6. (**1.0 ponto**) Existe algum tipo de hierarquia em relação aos critérios de teste estrutural, todos os nós, todos os arcos e todos os caminhos? Se sim, explique-a, considerando a perspectiva dos níveis de cobertura desejados.
R: Sim, existe uma hierarquia em relação ao nível e força de cobertura de casos de testes.
 - Todos os nós - exige que a execução do programa passe pelo menos uma vez em todos os nós/comandos e, portanto é o que possui menor cobertura de testes dos 3 critérios.
- Todos os arcos - executa o programa considerando todos os nós e arestas do grafo, passando por todos os desvios de fluxo do programa e, por isso, possui mais força de cobertura de testes do que o de Todos os nós.
 - Todos os caminhos - este exige que todos os caminhos possíveis do programa sejam executados, considerando nós, arestas e grafos, esgotando todas as possibilidades e, por isso, em relação ao nível de cobertura, este é o que apresenta o maior entre os 3. <font color=green>Certo.</font>

7. Considere a especificação, a seguir, de um hipotético programa que objetiva a classificação de um triângulo, a partir dos valores informados para os seus três lados.

   a) Dado um triângulo cujos segmentos medem A, B e C, que são números inteiros positivos na faixa de 0 a 100. Esse triângulo somente existirá se: (A + B < C) ou (A + C < B) ou (B + C < A).
   b) Quanto às medidas dos seus lados o triângulo, poderá ser classificado em:
         • Isósceles = quando possui dois lados com a mesma medida;
         • Escaleno = quando todos os seus lados têm medidas diferentes;
         • Equilátero = quando todos os lados tem a mesma medida;
         • Acutângulo = quando o quadrado de um dos seus lados é menor que a soma do quadrado dois outros dois. (A<sup>2</sup> < B<sup>2</sup> + C<sup>2</sup>).
         • Retângulo: quando o quadrado de um dos seus lados é igual à soma do quadrado dois outros dois. (A<sup>2</sup> = B<sup>2</sup> + C<sup>2</sup>).
         • Obtusângulo: quando o quadrado de um dos seus lados é maior que a soma do quadrado dois outros dois. A<sup>2</sup> > B<sup>2</sup> + C<sup>2</sup>.

7.1 (**2.0 pontos**) Definir uma tabela de decisão para o teste tanto da existência do triângulo, quanto para a definição do seu tipo. Consulte exemplo de tabela de decisão na tarefa 005.

OBS: Esta questão está com o enunciado errado!!

|Regras|R1|R2|R3|R4|R5|R6|R7|R8|R9|
|---|---|---|---|---|---|---|---|---|---|
|A+B>C ou A+C>B ou B+C>A|V|F|V|V|V|V|V|V|V|V|
|A = B|V|N/A|F|F|F|F|V|V|V|V|
|B = C|V|N/A|F|F|V|V|F|F|V|V|
|C = A|V|N/A|F|V|F|V|F|V|F|V|
|Não existe||x||||||||
|Equilátero|x|||||||||
|Isóceles||||x|x||x||||
|Escaleno|||x||||||||
|Não é possível||||||x||x|x|

<font color=green>Certo.</font>

7.2 (**2.0 pontos**) Criar os conjunto de casos de teste necessários para a cobertura das combinações constantes da tabela de decisão, seguindo o seguinte padrão:

|CT|Lado A|Lado B|Lado C|Resultado|
|---|---|---|---|---|
|01|5|5|5|Equilátero|
|02|10|3|3|Não existe|
|03|6|7|8|Escaleno|
|04|4|6|4|Isóceles|
|05|8|10|10|Isóceles|
|06|10|10|8|Isóceles|
|07|5|5|5|Equilátero|


<font color=orange>Parcialmente correto. Os casos de teste 01 e 07, são redundantes. Nota 1,8.</font>

INSTRUÇÕES:
1. Tipo: Prova individual;
2. Local de Entrega: Plataforma Turing
3. Forma de Entrega: Entregar este arquivo, editado com suas respostas, no formato .md, nominado da seguinte forma: ts2021-2_prova-p1_mat.md, onde mat deverá ser substituído pelo número da sua matrícula.
4. **Entrega diferente da especificada não será avaliada.**
5. Data da Entrega: 22/02/2022, as 23h59min.
6. Critério de Aceitação: arquivo entregue, conforme solicitado.
