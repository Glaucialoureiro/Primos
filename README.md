# Primos


//Trab 2: Numeros Primos
//Nome: Glaucia Loureiro
//Matrícula: 0050014804
//Professor: Alex Salgado

#include <stdio.h>

#include<stdlib.h>

int main()
{
    
    int num=0, cont = 0, i, opc=1;
    
    printf("Ola, meu nome eh Glaucia Loureiro e vou calcular numeros primos\n");
    
    while (opc<=1)
    {
        do
            
        {
            printf("\nEntre com um numero positivo:");
            
            scanf("%d", &num);
        }
        
        while(num<=0);
        {
        
            for (i=1; i<=num; i++)
            {
                if (num % i == 0)
                {
                    cont++;
                }
            }
        }
    if (cont==2)
        printf("\n%d eh um numero primo", num);
    
    else
        printf("\n%d NAO EH um numero primo", num);
            printf("\nDeseja continuar? Se sim digite 1, se n~ão digite 2:");
            scanf ("%d", &opc);
        cont = 0;
    }
    
    if (opc==2)
        
        printf("\nObrigada, ate a proxima! Para ver o meu codigo entre no link....");
    
    //system ("pause");
    return 0;
    
}


