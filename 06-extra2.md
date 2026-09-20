# Exercício Resolvido — Par ou Ímpar

## Enunciado
Escreva um programa em C que peça um número inteiro ao usuário e informe se ele é par ou ímpar.

## Solução

```c
#include <stdio.h>

int main() {
    int numero;

    printf("Digite um número inteiro: ");
    scanf("%d", &numero);

    if (numero % 2 == 0) {
        printf("%d é par.\n", numero);
    } else {
        printf("%d é ímpar.\n", numero);
    }

    return 0;
}
```

## Explicação passo a passo

1. `scanf("%d", &numero);` — lê o número digitado pelo usuário e armazena na variável `numero`. O `&` é necessário porque o `scanf` precisa do endereço de memória da variável, não do seu valor.
2. `numero % 2` — o operador `%` (módulo) retorna o resto da divisão de `numero` por 2.
3. Se o resto for `0`, o número é par; caso contrário, é ímpar.
4. O `if/else` decide qual mensagem imprimir com base nesse resultado.

## Teste
| Entrada | Saída esperada |
|---|---|
| 4 | 4 é par. |
| 7 | 7 é ímpar. |
| 0 | 0 é par. |