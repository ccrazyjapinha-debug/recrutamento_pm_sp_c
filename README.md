#include <stdio.h>

int main(){

    
    char sexo;
    char nome[20];
    int idade;
    float altura;

printf("\n========================\n");
printf("\n  BEM VINDO AO RECRUTAMENTO DA POLICIA MILITAR DE SP \n");
printf("\nPara comecar digite seu nome: ");
scanf("%s", nome);

printf("\nDigite sua idade: ");
scanf("%d", &idade);

printf("\nDigite sua altura: ");
scanf("%f", &altura);


printf("\nDigite seu genero(F/M): ");
scanf(" %c", &sexo);

if(sexo == 'm' || sexo == 'M'){
    if(idade >= 18 && idade <= 30 && altura > 1.65){
        printf("\nParabens voce atende aos requisitos para a pm de sp senhor %s!!!\n", nome);
    }
else {
    printf("\nDesculpa, voce nao atende aos nossos requisitos senhor %s", nome);}
    printf("\nAtendimento encerrado !");
}


else if(sexo == 'f' || sexo == 'F'){
    if(idade >= 18 && idade <= 30 && altura > 1.60){
        printf("\nParabens voce atende aos requisitos para a pm de sp senhor %s!!!\n", nome);
    }
        else{
        printf("\nDesculpe, mas senhorita %s nao atende aos nossos requisitos", nome);
    }
    }


return 0;
