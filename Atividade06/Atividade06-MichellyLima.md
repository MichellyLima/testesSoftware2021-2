## Tarefa 006 - 15/02/2022 - Grafo de Fluxo de Controle

1. Considere o fragmento de código implementado na Linguagem de Programação Java.

~~~java

public class Avaliacao {


1    public String avalia(double nota1, double nota2, int faltas, int cargaHoraria) throws ValoresInvalidosException{
2        String result;
3        double percentualFaltas = (faltas*100/cargaHoraria);
4        double media = (nota1 + nota2)/2;
5        if((nota1 < 0.0 || nota1 > 10) || (nota2 < 0.0 || nota2 > 10) || (faltas < 0 || faltas > cargaHoraria) || cargaHoraria < 0){
6            throw new ValoresInvalidosException();//result = "Valores Inválidos.";
7        }else if(percentualFaltas > 25.0){
8            result = "Reprovado por Falta.";
9        }else if(media < 3.0){
10            result = "Reprovado por Média.";
11        }else if(media >= 3.0 && media < 6.0){
12            result = "Prova Extra.";
13        }else{
14            result = "Aprovado.";
15        }
16        return result;
17    }
18 }
~~~

2. Pede-se:
   1. Desenhar o **Grafo do Fluxo de Controle**. Pode-se anexar a imagem, aqui neste arquivo.
   2. Calcular a complexidade ciclomática do código. Exemplo de coo calcular pode ser obtido no [link](https://www.treinaweb.com.br/blog/complexidade-ciclomatica-analise-estatica-e-refatoracao)
   3. Definir quantos caminhos de execução existem;
   4. Definir os casos de teste necessários para se percorrer todos estes caminhos. Cada caso de teste deve ter o valor correspondente para cada variável de entrada e o valor esperado.

INSTRUÇÕES:
1. Tipo: Tarefa Individual;
2. Local de Entrega: _branch main/master_ do repositório pessoal do aluno, criado para a manutenção do controle de versão dos artefatos da disciplina. O arquivo a ser entregue, pode ser este mesmo, editado com as respostas das questões solicitadas.
3. Data da Entrega: 21/02/2021, as 23h59min.
4. Critério de Aceitação: arquivo entregue, conforme solicitado.

#### RESPOSTAS

1. Desenhar o **Grafo do Fluxo de Controle**. Pode-se anexar a imagem, aqui neste arquivo.
![graph](https://user-images.githubusercontent.com/43323869/155046780-b850d049-91c7-485e-83f1-68cad4c6bb45.png)

2. Calcular a complexidade ciclomática do código. Exemplo de como calcular pode ser obtido no [link](https://www.treinaweb.com.br/blog/complexidade-ciclomatica-analise-estatica-e-refatoracao)
<br/>
V(G) = E – N + 2 - onde E é o número de arestas (setas) e N é o número de nós do grafo G.
<br/>
Dado que temos 27 arestas e 18 nós: 27 - 18 +2 = 11

3. Definir quantos caminhos de execução existem;

1-2-9 <br/>
1-2-3-9 <br/>
1-2-3-4-9 <br/>
1-2-3-4-5-9 <br/>
1-2-3-4-5-6-9 <br/>
1-2-3-4-5-6-7-9 <br/>
1-2-3-4-5-6-7-8-9 <br/>
1-2-3-4-5-6-7-8-10-11-18 <br/>
1-2-3-4-5-6-7-8-10-12-13-18 <br/>
1-2-3-4-5-6-7-8-10-12-14- 17-18 <br/>
1-2-3-4-5-6-7-8-10-12-14-15-16-18 <br/>
1-2-3-4-5-6-7-8-10-12-14-15-17-18

4. Definir os casos de teste necessários para se percorrer todos estes caminhos. Cada caso de teste deve ter o valor correspondente para cada variável de entrada e o valor esperado.

|Caso de Teste|nota1|nota2|falta|cargaHoraria|Resultado Esperado|
|--|--|--|--|--|--|--|
|01| nota1 = -1| N/A | N/A | N/A | "Valores Inválidos." |
|02|  nota1 = 12 | N/A | N/A | N/A | "Valores Inválidos." |
|03| nota1 = 7 | nota2 = -1 | N/A | N/A | "Valores Inválidos." |
|04| nota1 = 7 | nota2 = 12 | N/A | N/A | "Valores Inválidos." |
|05| nota1 = 7 | nota2 = 8 | faltas = -1 | N/A | "Valores Inválidos" 
|06| nota1 = 7 | nota2 = 8 | faltas = 2 | cargaHoraria = 0 | "Valores Inválidos." |
|07| nota1 = 7 | nota2 = 8 | faltas = 2 | cargaHoraria = -1 | "Valores Inválidos." |
|08| nota1 = 7 | nota2 = 8 | faltas = 25 | cargaHoraria = 100 | "Reprovado por falta." |
|09| nota1 = 2 | nota2 = 2 | faltas = 2 | cargaHoraria = 32 | "Reprovado por Média." |
|10| nota1 = 7 | nota2 = 3 | faltas = 2 | cargaHoraria = 32 | "Prova Extra." |
|11| nota1 = 7 | nota2 = 9 | faltas = 2 | cargaHoraria = 32 | "Aprovado." |
