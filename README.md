
# Sintaxe básica de C

## Comentários

```c
// Este é um comentário de linha, tudo que está comentado não é exetutado pelo programa

/*
Este é um comentário de bloco
que pode se estender por várias linhas
*/
```

## Inclusão de Bibliotecas

```c
#include <stdio.h> // Biblioteca de entrada e saída padrão
#include <stdlib.h> // Biblioteca padrão do sistema
```

## Função Principal

```c
int main() {
    // Código da função principal
    return 0;
}
```

## Tipos de Dados

```c
int inteiro;
float flutuante;
char caractere;
```

## Declaração de Variáveis

```c
int idade;
float altura;
char letra;
```

## Operadores Aritméticos

```c
+, -, *, /, %
```

## Estruturas de Controle

### Condicional

```c
if (condição) {
    // código
} else if (outra_condição) {
    // outro código
} else {
    // código alternativo
}
```

## Estrutura switch

A estrutura switch é usada para tomar decisões com base no valor de uma variável.

```c
int opcao = 2;

switch(opcao) {
    case 1:
        printf("A opção é 1\n");
        break;
    case 2:
        printf("A opção é 2\n");
        break;
    case 3:
        printf("A opção é 3\n");
        break;
    default:
        printf("Opção inválida\n");
}
```

No exemplo acima, se `opcao` for 1, ele imprimirá "A opção é 1". Se for 2, imprimirá "A opção é 2", e assim por diante. Se `opcao` não corresponder a nenhum dos casos, será executado o bloco de código dentro do `default`.

Essa é a estrutura básica do switch em C, utilizada para tomar decisões com base no valor de uma variável inteira.

---

## Entrada e Saída de Dados

### Saída (printf)

```c
int inteiro = 10;
float flutuante = 3.14;
char caractere = 'a';

printf("Inteiro: %d\n", inteiro);
printf("Flutuante: %f\n", flutuante);
printf("Caractere: %c\n", caractere);
```

### Entrada (scanf)

```c
int inteiro;
float flutuante;
char caractere;

printf("Digite um inteiro: ");
scanf("%d", &inteiro);

printf("Digite um flutuante: ");
scanf("%f", &flutuante);

printf("Digite um caractere: ");
scanf(" %c", &caractere); // Note o espaço antes de %c para consumir o caractere de nova linha

printf("Inteiro: %d\n", inteiro);
printf("Flutuante: %f\n", flutuante);
printf("Caractere: %c\n", caractere);
```

---


## Operadores Lógicos

```c
int a = 5, b = 3;

// E(AND) lógico
if (a > 0 && b > 0) {
    printf("Ambos a e b são maiores que zero\n");
}

// OU(OR) lógico
if (a == 5 || b == 5) {
    printf("Pelo menos um dos valores é igual a cinco\n");
}

// NEGAÇÃO(NOT) lógica
if (!(a == 0)) {
    printf("O valor de a não é zero\n");
}
```

Os operadores lógicos em C são `&&` (AND), `||` (OR) e `!` (NOT). Eles são usados para combinar condições em instruções condicionais.


## Resto da Divisão

```c
int resto = dividendo % divisor;
```

## Operadores de Repetição
### For

Inicialização: A primeira parte é executada apenas uma vez, no início do loop. Geralmente é usada para inicializar variáveis de controle. Por exemplo, int i = 0; inicializa a variável i com o valor 0.
Condição: A segunda parte é a condição que determina se o loop deve continuar executando. Enquanto essa condição for verdadeira, o loop continuará sendo executado. Por exemplo, i < 5; significa que o loop continuará enquanto o valor de i for menor que 5.
Incremento/Decremento: A terceira parte é executada após cada iteração do loop. Geralmente é usada para incrementar ou decrementar a variável de controle. Por exemplo, i++ incrementa o valor de i em 1 a cada iteração.



```c
#include <stdio.h>

int main() {
    int i;

    // Imprime os números de 1 a 5
    for (i = 1; i <= 5; i++) {
        printf("%d\n", i);
    }

    return 0;
}
```
