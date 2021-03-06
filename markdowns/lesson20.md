# Estruturas de Dados Homogêneas
---
+ Estrutura de dados Homogênea ou Matriz é uma coleção de variáveis de mesmo tipo, acessíveis com um único nome e armazenados contiguamente (um após o outro) na memória.

+ A individualização de cada variável é feita através do uso de índices.

+ Os Vetores são matrizes de uma só dimensão, isto é, necessita apenas 1 índice para acesso as variáveis. 

+ As Matrizes possuem mais de uma dimensão, isto é,  necessitam de um índice para cada dimensão para acesso as variáveis. 

+ A figura a seguir exibe a diferença entre declarar várias variáveis simples e uma variável do tipo Vetor. As variávies simples necessariamente são acessadas pelo seu nome enquanto que as variáveis que formam o vetor são acessadas através do nome do vetor mais um índice indicando sua posição na estrutura. 
 
![programa](/markdowns/vetor.gif)

---
Declaração de Vetores
---
        int Vetor[6];   /* declara um vetor do tipo int (números inteiros) de 6 posições */

        float Vetor[3]; /*declara um vetor do tipo float(números com casas decimais) com 3 posições */
        
        char Vetor[10] /* declara um vetor do tipo char com 10 posições  */

---
Mover valor para um vetor
---
+ Na linguagem C, os vetores tem o primeiro elemento na posição 0(zero). Assim, se tomarmos "K" como sendo o tamanho do vetor a última posição é a de índice "K-1". Por exemplo, um vetor de tamanho 10 (k=10) tem o seu último elemento na posição 9.
+ Exemplos de mover valor para uma matriz/vetor 
```
               Vetor[0] = 4; /*  Move o valor 4 para a primeira posição do "Vetor" */
               Vetor[4] = 8; /*  Move o valor 8 a quinta posição do "Vetor" (Não se esqueçam que a primeira é zero). */
               Vetor[1] = 15; /* Move o valor 15 para a segunda posição do "Vvetor" */
```
+ Para inicializar um vetor, isto é, mover valores para todos os elementos precisamos de uma estrutura de repetição. A estrutura de repetição <b>FOR</b> se adequa perfeitamente às Matrizes(vetores) porque a variável de controle da repetição pode ser usada para marcar as posições do vetor.
+ Por exemplo, mover o valor 100 para todas as posições de um vetor do tipo int de tamanho 5.
```
   for(i = 0; i < 5; i++)
   {
      vet[i] = 100;
    }
```
+ A figura abaixo exibe a execução do trecho de código acima:
![programa](/markdowns/movevetor.gif)
