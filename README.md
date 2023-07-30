# MediaC
The C Program calculates the mean or average of 6 numbers, to process and calculate the average value, the While loop is used until all the numbers have been processed for the calculation.
/*Calculo de la media de 6 numeros*/
#include <stdio.h>
#include <stdlib.h>
int main(int argc, char *argv[])
{   
    const int TotalNum = 6;
    int ContadorNum = 0;
    float SumaNum = 0;
    float media;

    printf("Introduzca %d numeros\n", TotalNum);

    while(ContadorNum < TotalNum) 
    {                                        /*Valores a Procesar*/
      float numero;
      scanf("%f", &numero);                  /* Leer siguiente numero*/ 
      SumaNum += numero;                     /* Anadir valor a Acumulador */
      ++ContadorNum;                         /* Incrementar numeros leidos  */
    }
    media = SumaNum/ContadorNum;
   printf("Media: %.2f \n", media);
   system("PAUSE");	
   return 0;

    }
