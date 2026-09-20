# Conceitos Fundamentais

Antes de programar, é importante entender alguns conceitos-base da Linguagem C.

## Estrutura básica de um programa em C

```c
#include <stdio.h>

int main() {
    printf("Olá, mundo!\n");
    return 0;
}
```

- `#include <stdio.h>`: importa a biblioteca padrão de entrada e saída.
- `int main()`: função principal, ponto de entrada de todo programa em C.
- `printf()`: exibe texto na tela.
- `return 0;`: indica que o programa terminou sem erros.

## Variáveis e tipos de dados

C exige que você declare o tipo de cada variável antes de usá-la:

```c
int idade = 20;        // números inteiros
float altura = 1.75;   // números decimais
char inicial = 'A';    // um único caractere
```

Principais tipos: `int`, `float`, `double`, `char`.

## Operadores

- Aritméticos: `+`, `-`, `*`, `/`, `%`
- Relacionais: `==`, `!=`, `>`, `<`, `>=`, `<=`
- Lógicos: `&&`, `||`, `!`

## Estruturas de controle

**Condicionais:**
```c
if (idade >= 18) {
    printf("Maior de idade\n");
} else {
    printf("Menor de idade\n");
}
```

**Laços de repetição:**
```c
for (int i = 0; i < 5; i++) {
    printf("%d\n", i);
}
```

## Funções

Blocos de código reutilizáveis:

```c
int soma(int a, int b) {
    return a + b;
}
```

## Próximo passo
Com esses conceitos em mãos, siga para o módulo de exercícios práticos.