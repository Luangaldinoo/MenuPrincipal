#include <stdio.h>
int main()
{
   int tentativas = 0;
   int senha;
   int opcao = 0;

       while (tentativas < 3)
   {
      printf("\nDigite a senha:  ");
      scanf("%d", &senha);

      if (senha == 2005)
      {
         printf("Acesso liberado!\n");
         break;
      }
      else
      {
         printf("Acesso negado, tente novamente em instantes");
         tentativas++;
      }
      if (tentativas == 3)
      {
         printf(" Limite de tentativas atingido! tente novamente em 10min ");
      }
   }

   while (opcao != 3)
   {
      printf("\n\n=== MENU PRINCIPAL ===\n");
      printf("1- Falar com alessia (atendente)\n");
      printf("2- Mostrar Informacoes\n");
      printf("3- Sair\n");
      printf("Escolha uma opcao:   ");
      scanf("%d", &opcao);

      if (opcao == 1)
      {
         printf(" Oi, sou alessia! Em que posso ajudar \n");
         break;
      }
      else if (opcao == 2)
      {
         printf(" Funcionamos de 17h as 00\n");
         break;
      }
      else if (opcao == 3)
      {
         printf(" Saindo... Até mais!\n");
         break;
      }
      else
         {
             printf(" Comando Invalido, tente novamente!!");
             break;
         }
   }
   return 0;
}
