## Tarefa 004 - 19/01/2022 - Análise do Valor Limte - Definição de casos de testes.

**DEFINIÇÃO**:
1. Considerando o conjunto de classes de equivalência que você definiu em atendimento à **Tarefa 003 - 21/12/2021 - Definição de Classes de Equivalência**.
2. Considerando as explicações a respeito do critério de teste funcional **Análise do Valor Limite** disponíveis em:
   1. [Análise do Valor Limite 1](https://viniciuspessoni.com/2020/03/15/analise-do-valor-limite/).
   2. [Análise do Valor Limite 2](https://www.youtube.com/watch?v=EQU5ODvmwzs).
   3. [Análise do Valor Limite 3](https://www.youtube.com/watch?v=jX7uyaTAn-k).
3. Pede-se a definição do conjunto de casos de testes necessários para o teste do mesmo cenário descrito na tarefa 003. Estes casos de teste deverão ser criadas a partir das diretrizes definidas pelo critério funcional "Análise do Valor Limte".
4. O Conjunto de casos de testes derivado deve seguir o seguinte padrão:

|CT|Valor de Entrada|Resultado Esperado|Classe Equivalência|
|--|--|--|--|
|CT01|nota01 = -2.00|Valor Inválido|CE1|
|CT02|nota01 = 0.00|Valor Válido|CE2|
|CT03|nota01 = 1.10|Valor Válido|CE2|
|CT04|nota02 = -1.00|Valor Inválido|CE3|
|CT05|nota02 = 0.00|Valor Válido|CE4|
|CT06|nota02 = 1.01|Valor Válido|CE4|
|CT07|cargaHoraria = 0|Valor Inválido|CE5|
|CT08|cargaHoraria = -2|Valor Inválido|CE6|
|CT09|cargaHoraria = 3|Valor Válido|CE6|
|CT10|faltas = -1|Valor Inválido|CE7|
|CT11|faltas = 0|Valor Válido|CE8|
|CT12|faltas = 3|Valor Válido|CE8|

Onde:
**CT** = Caso de Teste, seguido de um valor sequencial;
**Valor de entrada** é o valor informado para a variável;
**Resultado esperado** é o resultado que se espera da execução da função;
**Classe de Equivalência** é a identificação de qual classe de equivalência está sendo exercitada pelo caso de teste.

INSTRUÇÕES:
1. Tipo: Esta tarefa é individual;
2. Como responder: Pode-se editar este arquivo, complementando as tabelas de definições de classes de equivalência e dos casos de teste.
3. Local de Entrega: A entrega deverá seu repositório pessoal, utilizado para a manutenção dos artefatos de trabalho da disciplina (ts-2021-2);
4. Data da Entrega: Esta tarefa deve estar disponível para avaliação até o dia 24/01/2022 às 23h59min.
5. Esta tarefa valerá nota e presença para aula assíncrona do dia 18/01/2022.
6. Critério de Aceitação: tarefa entregue conforme especificado e na data definida.
7. Caso necessite de suporte, pode encaminhar mensagem para o professor.