# Operações com Ponteiros

+ Um ponteiro pode ter o valor especial <b>NULL</b> que é o "zero" (aponta para nenhum endereço) de ponteiros.
    <p>Exemplo</p>
        <b>int *p = NULL;</p>

---
Atribuição
---
+ O ponteiro <b>ptr1</b> aponta para a mesma variável (endereço) que o ponteiro <b>ptr</b>.
```C runnable
#include <stdio.h>
int main(){
int *ptr, *ptr1;
int numero;
numero = 20;
ptr = &numero;
ptr1 = ptr; // ambos estão apontado para o endereço de número.
printf("\nptr = %d",*ptr);
printf("\nptr1 = %d",*ptr1);
}
```
+ a variável apontada por <b>ptr1</b> recebe o mesmo conteúdo da variável apontada por <b>ptr</b>;
```C runnable
#include <stdio.h>
int main(){
int *ptr, *ptr1;
int numero, total;
numero = 20;
total = 10;
ptr = &numero;
ptr1 = &total;
*ptr1 = *ptr; // as variáveis numero e total contém o mesmo valor de número.
printf("\nNumero = %d",numero);
printf("\nTotal = %d",total);
}
```
+ Apenas duas operações aritméticas podem ser utilizadas com ponteiros: adição e subtração. Muito util para trabalhar com vetores.
+ Podemos somar e subtrair apenas valores <b>INTEIROS.</b>

``` 
p++; 
soma +1 no endereço armazenado no ponteiro. 
p--; 
subtrai 1 no endereço armazenado no ponteiro. 
```

+ Com relação ao conteúdo apontado, valem todas as operações
```
(*p)++; 
incrementar o conteúdo da variável apontada pelo ponteiro p;
*p = (*p) * 10; 
multiplica o conteúdo da variável apontada pelo ponteiro p por 10;
```

+ Operações relacionais
```
== e !=        para saber se dois ponteiros são iguais ou diferentes. 
>, <, >= e <=  para saber qual a posição (endereço) mais alta na memória ocupado por um ponteiro.
```

