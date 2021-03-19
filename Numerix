#include <stdlib.h>
#include <stdio.h>
#include <string.h>
#include <time.h>

#define MAX_FACIL 15
#define MAX_MEDIO 10
#define MAX_DIFICIL 5
#define PONTOS_INICIAIS 1000

int vamosdenovo(void){//Fun��o para que o jogo volte a ser executado caso o usu�rio deseje;
    char s; //necessario para iniciar o loop com confirma��o sim;

    printf("\n\n\t\tVAMOS DE NOVO? [s/n]: ");
    fflush(stdin);
    scanf("%s", &s);

        if (s == 's'){
        system("CLS");
        return main();
        }else{
        if(s== 'n'){
        printf("\n\t\tTCHAU!");
        return 0;
        }else{
            printf("\n\t\tCOMANDO INVALIDO, PORFAVOR ESCOLHA [s/n]\n\t\tEM LETRA MINUSCULA, VEJA SE O CAPSLOCK ESTA ATIVADO.\n");
            return vamosdenovo();
            }
        }
}

int main(){
    int num,x ; //numero digitado pelo usu�rio
    int pont, nivel; //pontua��o do usu�rio.
    int tentativa=1, j=0; //numero de tentatativas, vai ser contado no final, j=auxiliar na contagem dee tentativas
    int r1, r2; //resposta a primeira pergunta
    char s; //necessario para iniciar o loop com confirma��o sim
    //float tentativas[100];
    srand(time(NULL));
    x = rand() % 100 + 1; //fun��o rand para gerar numeros aleat�rios


    printf("\n\t\t[===============(-*-*-)==============]\n");
    printf("\t\t[                 OI!                ]\n");
    printf("\t\t[Vamos jogar um jogo de adivinhacao? ]\n");
    printf("\t\t[===============(-*-*-)==============]\n\n");
    printf("\t\t        =>[1] sim ou nao[2]<= \n\t\t\t\t");
    scanf("%d", &r1);

        if(r1 == 1){
        system("CLS");
        printf("\t\tEscolha o nivel que vc deseja jogar:\n");
        printf("\t\t[1] FACIL\n\t\t[2] MEDIO\n\t\t[3] DIFICIL\n\t\t");
        scanf("%d", &nivel);
        system("CLS");

            if(nivel==1){
                printf("\n\n\tVOCE TEM 15 TENTATIVAS PARA ACERTAR MEU NUMERO DE 0 A 100!\n\t\t\t\tTA FACIL!\n");
                for(tentativa=1; tentativa<=MAX_FACIL; tentativa++){
                printf("\n\t\tVAMOS LA! CHUTE %d DE %d \n",tentativa, MAX_FACIL);
                printf("\n\t\tESCOLHA UM NUMERO: ");
                scanf("%d",&num);

                if(num == j){
                    printf("\n\t\t NUMERO REPETIDO! TENTE OUTRO NUMERO!\n");
                    tentativa--;//Assim a tentativva vai decrescendo diminue um valor do que acumulou antes, ficando no mesmo lugar;
                }
                if (num < x){
                    printf("\t\tAcho que o numero eh maior que %d\n", num);
                }else {
                if(num > x){
                    printf("\t\tQue tal tentar um numero menor %d\n", num);
                }else {
                if(num == x){
                    system("CLS");

                    printf("\n\t\t[===============(-*-*-)==============]\n");
                    printf("\t\t[           Acertou Miseravi!        ]\n");
                    printf("\t\t[      Numero de tentativas: %d       ]\n", tentativa);
                    printf("\t\t[         O numero era: %d           ]\n", x);

                    pont = abs((PONTOS_INICIAIS - tentativa) - x)/2;//Calculo dos pontos;

                    printf("\t\t[     Sua pontuacao foi de: %d      ]\n", pont);
                    printf("\t\t[===============(-*-*-)==============]\n\n");
                    vamosdenovo();
                    break;//Necess�rio para impedir a contagem de continua funcionano at� que tentativa >= max;
                    }
                }
                }
                j=num;

                if (tentativa >= MAX_FACIL) {
                system("CLS");
                printf("\n\t\t[===============(-*-*-)==============]\n");
                printf("\t\t[         NAO FOI DESSA VEZ!         ]\n");
                printf("\t\t[          O numero era: %d          ]", x);
                printf("\n\t\t[===============(-*-*-)==============]\n");
                vamosdenovo();
                break;
              }
            }
        }

            if(nivel==2){
                printf("\n\tVOCE TEM 10 TENTATIVAS PARA ACERTAR MEU NUMERO DE 0 A 100!\n\t\t\tTA MAIS OU MENOS!\n");
                for(tentativa=1; tentativa<=MAX_MEDIO; tentativa++){
                printf("\n\t\tVAMOS LA! CHUTE %d DE %d \n",tentativa, MAX_MEDIO);
                printf("\n\t\tESCOLHA UM NUMERO: ");
                scanf("%d",&num);

                if(num == j){
                    printf("\n\t\t NUMERO REPETIDO! TENTE OUTRO NUMERO!\n");
                    tentativa--;//Assim a tentativva vai decrescendo diminue um valor do que acumulou antes, ficando no mesmo lugar;
                }
                if (num < x){
                    printf("\t\tAcho que o numero eh maior que %d\n", num);
                }else {
                if(num > x){
                    printf("\t\tQue tal tentar um numero menor %d\n", num);
                }else {
                if(num == x){
                    system("CLS");
                    printf("\n\t\t[===============(-*-*-)==============]\n");
                    printf("\t\t[           Acertou Miseravi!        ]\n");
                    printf("\t\t[      Numero de tentativas: %d       ]\n", tentativa);
                    printf("\t\t[         O numero era: %d           ]\n", x);

                    pont = abs((PONTOS_INICIAIS - tentativa) - x)/2;//Calculo dos pontos;

                    printf("\t\t[     Sua pontuacao foi de: %d      ]\n", pont);
                    printf("\t\t[===============(-*-*-)==============]\n\n");
                    vamosdenovo();
                    break;//Necess�rio para impedir a contagem de continua funcionano at� que tentativa >= max;
                    }
                }
                }
                j=num;

                if (tentativa >= MAX_MEDIO) {
                system("CLS");
                printf("\n\t\t[===============(-*-*-)==============]\n");
                printf("\t\t[         NAO FOI DESSA VEZ!         ]\n");
                printf("\t\t[          O numero era: %d          ]", x);
                printf("\n\t\t[===============(-*-*-)==============]\n");
                vamosdenovo();
                break;
              }
            }
        }

            if(nivel==3){
                printf("\n   VOCE TEM 5 TENTATIVAS PARA ACERTAR MEU NUMERO DE 0 A 100. EH DIFICIL VIU!\n\t\t   . . . MAS NAO IMPOSSIVEL\n");
                for(tentativa=1; tentativa<=MAX_DIFICIL; tentativa++){
                printf("\n\t\tVAMOS LA! CHUTE %d DE %d \n",tentativa, MAX_DIFICIL);
                printf("\n\t\tESCOLHA UM NUMERO: ");
                scanf("%d",&num);

                if(num == j){
                    printf("\n\t\t NUMERO REPETIDO! TENTE OUTRO NUMERO!\n");
                    tentativa--;//Assim a tentativva vai decrescendo diminue um valor do que acumulou antes, ficando no mesmo lugar;
                }
                if (num < x){
                    printf("\t\tAcho que o numero eh maior que %d\n", num);
                }else {
                if(num > x){
                    printf("\t\tQue tal tentar um numero menor %d\n", num);
                }else {
                if(num == x){
                    system("CLS");
                    printf("\n\t\t[===============(-*-*-)==============]\n");
                    printf("\t\t[           Acertou Miseravi!        ]\n");
                    printf("\t\t[      Numero de tentativas: %d       ]\n", tentativa);
                    printf("\t\t[         O numero era: %d           ]\n", x);

                    pont = abs((PONTOS_INICIAIS - tentativa) - x)/2;//Calculo dos pontos;

                    printf("\t\t[     Sua pontuacao foi de: %d      ]\n", pont);
                    printf("\t\t[===============(-*-*-)==============]\n\n");
                    vamosdenovo();
                    break;//Necess�rio para impedir a contagem de continua funcionano at� que tentativa >= max;
                    }
                }
                }
                j=num;

                if (tentativa >= MAX_DIFICIL) {
                system("CLS");
                printf("\n\t\t[===============(-*-*-)==============]\n");
                printf("\t\t[         NAO FOI DESSA VEZ!         ]\n");
                printf("\t\t[          O numero era: %d          ]", x);
                printf("\n\t\t[===============(-*-*-)==============]\n");
                vamosdenovo();
                break;
              }
            }
        }

    }else{
        printf("\n\n\t\t\t-> QUE PENA <-\n");
        printf("\n\t\t\t      :'-( ");
        }

    return 0;
    }
