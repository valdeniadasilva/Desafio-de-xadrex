# Desafio-de-xadrex
#include <stdio.h>

// Função para mover a Torre usando um loop for
void moverTorre(int casas) {
    printf("Movimento da Torre:\n");
    for (int i = 1; i <= casas; i++) {
        printf("Movendo para frente %d casa(s)\n", i);
    }
}

// Função para mover o Bispo usando um loop while
void moverBispo(int casas) {
    printf("\nMovimento do Bispo:\n");
    int i = 1;
    while (i <= casas) {
        printf("Movendo diagonalmente %d casa(s)\n", i);
        i++;
    }
}

// Função para mover a Rainha usando um loop do-while
void moverRainha(int casas) {
    printf("\nMovimento da Rainha:\n");
    int i = 1;
    do {
        printf("Movendo na horizontal %d casa(s)\n", i);
        i++;
    } while (i <= casas);
}

int main() {
    int casas = 5; // Número de casas que cada peça se moverá

    moverTorre(casas);
    moverBispo(casas);
    moverRainha(casas);

    return 0;
}