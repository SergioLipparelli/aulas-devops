# aulas-devops
//Opção de menu

#include<stdio.h>
int main(void){
    float soma=0;
    float valor;
    int opcao;
    do{
        printf("\n Escolha a opção do menu:");
        printf("\n 1. Deposito");
        printf("\n 2. Saque");
        printf("\n 3. Saldo");
        printf("\n 4. Sair");
        printf("\n Informe uma opção:");
        scanf("%d", &opcao);
        
    switch(opcao) {
        case 1:
        printf("\n Informe o Valor:");
        scanf("%f", &valor);
        soma += valor;
        break;
        
        case 2:
        printf("\n Informe o Valor para Saque:");
        scanf("%f", &valor);
        soma -= valor;
        break;
        
        case 3:
        printf("\n Seu Saldo disponivel = R$ %.2f", soma);
        break;
        
        case 4:
        printf("\n Saindo...");
        break;
        
        default:
        printf("\n Opção invalida");
     }
    }
    while (opcao != 4);
    printf("\n\n Fim das Operações!");
    
    return 0;
}
