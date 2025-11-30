#include <stdio.h>

int somaRecursiva(int a, int b) {
    if (b == 0) {
        return a;
    }
    return somaRecursiva(a + 1, b - 1);
}

int main() {
    int x, y;

    printf("Digite o primeiro valor: ");
    scanf("%d", &x);

    printf("Digite o segundo valor: ");
    scanf("%d", &y);

    int resultado = somaRecursiva(x, y);

    printf("Resultado da soma recursiva: %d\n", resultado);

    return 0;
}
