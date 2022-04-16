<div align=center>
  <img src="brasaooficialcolorido.png">
</div>

#### <p style="text-align: center;">Universidade Federal de Goiás</p>
#### <p style="text-align: center;">Instituto de Informática</p>
#### <p style="text-align: center;">Bacharelado em Engenharia de Software</p>
#### <p style="text-align: center;">Teste de Software - 2021/2</p>
#### <p style="text-align: center;">Gilmar Ferreira Arantes</p>
####  <p style="text-align: center;"> Prova P2 - 12/04/2022</p>

Matrícula: 201802780

Nome: Michelly Silva Lima

<font color="green">Nota 6,0</font>


1. Quanto ao Processo de Teste de Software, responda as duas questões seguintes:
   1. (**0,5 ponto**) Defina os seguintes conceitos Processo de Teste de Software, Projeto de Teste de Software e Plano de Teste de Sofware.
   R: O Processo de Teste de Software é um conjunto estruturado de etapas, atividades, artefatos, papéis e as responsabilidades com o objetivo de realizar os testes de software. O Projeto de Teste, por sua vez, descreve a estrutura dos elementos de testes e a realização dos casos de teste. Por fim, o Plano de Teste de Software é um documento com uma abordagem sistemática para o teste, detalhando o fluxo de trabalho durante o processo.
   <font color="red">Nota 0,5</font>
   2. (**0,5 ponto**) Descreva o relacionamento existente entre estes conceitos.
   R:O Processo de Teste é realizado para um Projeto de Teste, e contém em uma de suas etapas a elaboração de um Plano de Teste de Software, que este processo irá seguir para o projeto específico. <font color="red">Nota 0,5</font>
2. (**1,0 pontos**) Descreva as vantagens para a equipe de desenvolvimento ao se adotar um processo de teste ágil.
   R:Antecipar erros e bugs, garantir uma colaboração de todo o time de desenvolvimento no atingimento da qualidade do software, retirando a responsabilidade apenas do testador e assim podendo atingir a entrega de valor de forma mais rápida para o cliente.<font color="red">Nota 1,0</font>
3. (**1,0 ponto**) Cite pelo menos três características do Teste Exploratório.
   R:Não possui planejamento avançado, gera a documentação de teste conforme é realizada e é realizada pelo testador com o papel de usuário final.<font color="red">Nota 1,0</font>
4. Considere os arquivos .java (Banco.java, Agencia.java, Conta.java e BankValidator.java). Nos próprios arquivos .java estão definidas as regras para cadastramento de cada um deles (Banco, Agencia e Conta). Desta forma, pede-se:
   4.1. (**2.0 Pontos**) Definir os cenários de teste suficientes para testar o cadastro e movimentações financeiras envolvendo bancos, agências e contas, conforme especificado. Para cada cenário definir os critérios de teste adequados à definição dos seus casos de teste.

   | CE | Descrição | Critério de teste |
   |---|---|---|---|
   |01| criar banco com número fracionário | Partição de equivalência |
   |02| criar banco com número de 2 dígitos | Análise de Valor Limite |
   |03| criar banco com número de 4 dígitos | Análise de Valor Limite |
   |04| criar banco com nome de 4 dígitos | Análise de Valor Limite |
   |05| criar banco com nome de 101 dígitos | Análise de Valor Limite |
   |06| criar agência com número de 2 dígitos | Análise de Valor Limite |
   |07| criar agência com número de 6 dígitos | Análise de Valor Limite |
   |08| criar agência com nome de 4 dígitos | Análise de Valor Limite |
   |09| criar agência com nome de 101 dígitos | Análise de Valor Limite |
   |10| criar agência com cidade de 4 dígitos | Análise de Valor Limite |
   |11| criar agência com cidade de 101 dígitos | Análise de Valor Limite |
   |12| criar conta com 5 dígitos | Análise de Valor Limite |
   |13| criar conta com 7 dígitos | Análise de Valor Limite |
   |14| criar conta com tipo diferente de Poupança ou Corrente | Partição de equivalência |
   |15| sacar um valor maior que o saldo em Conta Corrente | Partição de equivalência |
   |16| sacar um valor maior que o saldo em Conta Poupança | Partição de equivalência |
   |17| depositar em conta Corrente e Poupança | Partição de equivalência |
   |18| transferência entre contas de valor menor que o saldo | Partição de equivalência |
   |19| transferência entre contas de valor maior que o saldo | Partição de equivalência |
   |20| creditar rendimentos em Conta Corrente | Partição de equivalência |
   |21| debitar juros de cheque especial em Conta Corrente | Partição de equivalência |
   |22| creditar rendimentos em Conta Poupança | Partição de equivalência |
   |23| debitar juros de cheque especial em Conta Poupança | Partição de equivalência |
   |24| criar banco válido | Partição de equivalência |
   |25| criar agência válida | Partição de equivalência |
   |26| criar conta válida | Partição de equivalência |

   <font color="red">Nota 1,5</font>

   4.2. (**2.0 Pontos**) Definir os casos de teste suficientes para a cobertura do teste de cada um dos cenários definidos. Documentar os casos de teste no seguinte padrão:

   |CT|Valores de Entrada|Resultado esperado|CE|
   |---|---|---|---|
   |CT01|1,24|banco não cadastrado|CE01|
   |CT02|11|banco não cadastrado|CE02|
   |CT03|1234|banco não cadastrado|CE03|
   |CT04|nome|banco não cadastrado|CE04|
   |CT05|loremipsumdolorsitametajklhflasnfwelofbalkedgfhskdbfsnfalloremipsumdolorsitametajklhflasnfwelofbalked|banco não cadastrado|CE05|
   |CT06|11|banco não cadastrado|CE06|
   |CT07|123456|agência não cadastrada|CE07|
   |CT08|tatu|agência não cadastrada|CE08|
   |CT09|loremipsumdolorsitametajklhflasnfwelofbalkedgfhskdbfsnfalloremipsumdolorsitametajklhflasnfwelofbalked|agência não cadastrada|CE09|
   |CT10|tatu|agência não cadastrada|CE10|
   |CT11|loremipsumdolorsitametajklhflasnfwelofbalkedgfhskdbfsnfalloremipsumdolorsitametajklhflasnfwelofbalked|agência não cadastrada|CE11|
   |CT12|12345|conta não cadastrada|CE12|
   |CT13|1234567|conta não cadastrada|CE13|
   |CT14|"Unicornio"|conta não cadastrada|CE14|
   |CT15|valor= 300 limite= 300 e saldo= 0, tipo: Corrente|saque realizado, cheque especial = 300|CE15|
   |CT16|valor= 300 limite= 300 e saldo= 0, tipo: Poupanca|saque não realizado|CE16|
   |CT17|depositar 500, saldo = 0 |saldo = 500|CE17|
   |CT18|valor= 50, saldo= 100|transferência realizada|CE18|
   |CT19|valor= 500, saldo= 100|transferência não realizada|CE19|
   |CT20|valor=800 | não realizado | CE20 |
   |CT21|valor=800 | não realizado | CE21 |
   |CT22|valor=800 | adicionado 800 ao saldo | CE22 |
   |CT23|valor=800 | retirado 800 do saldo | CE23 |
   |CT24|numero=123, nome="Santander"|CE24|
   |CT25|numero=1234, nome="Agencia cofrinho", cidade="Varginhas"|CE25|
   |CT26|numero= 123456, tipo="Corrente", agenciaValida | conta criada | CE26 |

   <font color="red">Nota 1,5</font>

   4.3. (3.0 Pontos) Implementar (na linguagem de programação java) as classes para o teste da criação dos objetos e das movimentações financeiras envolvendo bancos e agências e contas.

   <p><font color="red">Nota 0,0, os arquivos enviados são os mesmos compartilhados pelo professor. Não foram enviadas classes de teste.</font></p>

INSTRUÇÕES:
1. Tipo: Prova individual;
2. Local de Entrega: Plataforma Turing.
3. Forma de Entrega: arquivo compactado contendo:
   1. Este arquivo md, respondido.
   2. Classes de teste para (BancoTest, AgenciaTest e ContaTest);
   3. O arquivo compactado deverá ter o seguinte nome prova_p2<mat>.zip, onde mat é o número da matrícula do aluno(a).
4. Data da Entrega: 12/04/2022, as 22hs.
5. Critério de Aceitação: arquivo entregue, conforme solicitado.
6. Obs: segue no mesmo pacote o arquivo "org.apache.commons.lang.StringUtils", que é uma dependência do projeto. É deve ser inserida no _classpath_ do projeto de implementação da questão 4, caso não esteja utilizando o _maven_.
