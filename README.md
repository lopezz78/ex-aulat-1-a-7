# ex-aulat-1-a-7
/*Escrever um algoritmo que leia uma quantidade desconhecida de
números e conte quantos deles estão nos seguintes intervalos:
[0.25], [26,50], [51,75] e [76,100]. A entrada de dados deve
terminar quando for lido um número negativo.*/




#include <stdlib.h>
#include <stdio.h>
#include <locale.h>

int main()
{
    setlocale(LC_ALL,"portuguese");

    int num, a=0, b=0, c=0, d=0 ;


    do
    {
        printf("\n\tDigite um número de 1 a 100: ");
        scanf("%d", &num);

        if(num<0)
        {
            printf("\n\t0 a 25: %d\n\t26 a 50: %d\n\t51 a 75: %d\n\t76 a 100: %d", a, b, c, d);
        }


        if (num>=0 && num<26)
        {

            a++;
        }

        if (num>=26 && num<51)
        {

            b++;
        }

        if (num>=51 && num<76)
        {

            c++;
        }

        if (num>=75 && num<101)
        {

            d++;
        }

    }while (num>0);

}
