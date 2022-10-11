// CaixaEletronico-c-

#include <stdio.h>//biblioteca para habilitar (I/O)
#include<unistd.h>//biblioteca para a funcao sleep
#include <stdlib.h>//biblioteca que chama o system("cls");(LIMPA TELA)
//system("cls"); OU system("clear"); dependendo de onde vai compilar
int main (void)//funcao principal(main)
{
  int resp;//variavel de controle opcao(ficar / sair)
  int senha;//variavel para armazenar senha digitada
  float saldo = 100.00;

  int saque = 1;//opcao SAQUE no MENU
  float valorSaque;//armazena valor solicitado no SAQUE

  int deposito = 2;//opcao DEPOSITO no MENU
  int valorDeposito;//armazena valor DEPOSITADO

  int transferencia = 3;//opcao TRANSFERENCIA no MENU
  float valorTransferencia;//armazena valor solicitado na TRANSFERENCIA

  int sair = 0;//opcao SAIR no MENU
  int opcao;//armazena valor solicitado no MENU

  int x, y, z;//(x)e(y)armaxena agencia e conta; (z)armazena opcao proseguir ou corrigir
  int tempo =2;//controle de tempo sleep
  printf ("\n Entre com a senha: ");//solicita a senha da conta
  scanf ("%d", &senha);//armazena na variavel senha

  if (senha == 0000)//compara se a senha digitada e igual a '0000'
    {
      printf("\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\n");//emite som  
      system ("clear");//limpa a tela
      do//inicio do laco (do)
	    {
    	  printf ("\n ******* MENU *******");
    	  printf ("\n --------------------");//MENU DA CONTA
    	  printf ("\n SALDO R$ %.2f", saldo);
    	  printf ("\n --------------------");
    	  printf ("\n ********************");
    	  printf("\n");
    	  printf ("\n --------------------");
    	  printf ("\n '1'     SAQUE       ");
    	  printf ("\n --------------------");
    	  printf ("\n '2'    DEPOITO      ");
    	  printf ("\n --------------------");
    	  printf ("\n '3' TRANSFERENCIA   ");
    	  printf ("\n --------------------");
    	  printf ("\n '0'     SAIR        ");
    	  printf ("\n --------------------");
    	  printf("\n");
    	  printf ("\n ********************");
    	  printf ("\n ESCOLHA A OPCAO:  "  );
    	  scanf ("%d", &opcao);

          if (opcao == 1)//menu saque
	        {
	          printf("\7\7\7\7\7\7\7\7\7\7\7\n");//emite som
	          system ("clear");//limpa a tela
	          printf ("\n Digite valor do saque: ");
	          scanf ("%f", &valorSaque);//armazena valor digitado na variavel valorSaque

	          if (valorSaque <= saldo)//se valorSaque for menor ou igual ao saldo
	        	{
	        	 printf ("\n Aguarde**************");
    	         printf ("\n *********************");
    	         sleep (tempo);//comando delay para simular processamento interno
    	         printf("\7\7\7\7\7\7\7\7\7\7\7\n");//emite som
		         printf ("\n Saque de R$ %.2f realizado com sucesso",valorSaque);
		         saldo = (saldo - valorSaque);//subtrai do saldo o valor do saque
		         printf ("\n Seu saldo e R$ %.2f", saldo);//moetra na tel o que sobrou
        		 //--------------------------------------------------------------------------
        		 printf ("\n ****************************************");
        		 printf ("\n '1'(continuar) '2'(sair): ");
        		 scanf ("%d", &resp);//armazena valor lido na variavel resp
        		 printf("\7\7\7\7\7\7\7\7\7\7\7\n");//emite som
        		 system("clear");//limpa tela
        		 //em (do while) em quanto while(==1)o programa vai execultar o laco (do)
        		 //se o usuario escolher '2' while deixa de ser verdadeiro e sai do laco (do)
        		 //-------------------------------------------------------------------------------------
		        }
	            else 
	               if (valorSaque > saldo)//senao se valor saque for maior que o saldo
		             {
		               printf ("\n Saldo insuficiente!!!");
		               printf ("\n seu saldo é de R$ %.2f", saldo);
		                for(int i=0;i<=2;i++)
		                 {
		                  printf("\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\n");//emite som
		                  sleep(1);
		                 }
            		  //--------------------------------------------------------------------------
            		   printf ("\n ****************************************");
            		   printf ("\n '1'(continuar) '2'(sair): ");
            		   scanf ("%d", &resp);
            		   printf("\7\7\7\7\7\7\7\7\7\7\7\n");//emite som
            		   system("clear");
            		  //-------------------------------------------------------------------------------------
            		 }
	         }
          if(opcao == 2)//menu deposito
    	    {
    	      printf("\7\7\7\7\7\7\7\7\7\7\7\n");//emite som
    	      system ("clear");//limpa a tela
    	      printf ("\n Digite o valor a ser depositado: ");
    	      scanf ("%d", &valorDeposito);
    	      printf ("\n Aguarde**************");
    	      printf ("\n *********************");
    	      sleep (tempo);
    	      saldo = (saldo + valorDeposito);
    	      printf("\7\7\7\7\7\7\7\7\7\7\7\n");//emite som
    	      printf ("\n Deposito realizado com sucesso");
    	      printf ("\n Seu saldo e de R$ %.2f", saldo);
    	      //--------------------------------------------------------------------------
    	      printf ("\n ****************************************");
             printf ("\n '1'(continuar) '2'(sair): ");
              scanf("%d", &resp);
              printf("\7\7\7\7\7\7\7\7\7\7\7\n");//emite som
              system("clear");
             //-------------------------------------------------------------------------------------
    	    }
          if (opcao == 3)//menu transferencia CASO atenda requisutos
    	    {
    	      printf("\7\7\7\7\7\7\7\7\7\7\7\n");//emite som
    	      system("clear");
    	      printf ("\n Informe Agencia");
    	      printf ("\n (Ex: 1234)");
    	      printf ("\n: ");
    	      scanf ("%d", &x);
    	      printf ("\n Informe a conta com digito");
    	      printf ("\n (EX: 123456)");
    	      printf ("\n: ");
    	      scanf ("%d", &y);
    	      printf ("\n Informe valor R$: ");
    	      scanf ("%f", &valorTransferencia);
    	      system("clear");
    	      printf("\7\7\7\7\7\7\7\7\7\7\7\n");//emite som
    	      printf ("\n Agencia_Conta");
    	      printf ("\n    %d_%d   ", x, y);
    	      printf ("\n R$ %.2f", valorTransferencia);
    	      printf ("\n Confirmar transferencia ?");
    	      printf("\7\7\7\7\7\7\7\7\7\7\7\n");//emite som
    	      printf ("\n 1(Sim), 2(Corrigir)");
    	      scanf ("%d", &z);
    	      system("clear");
    	      if (z == 1)
    		   {
		        if (valorTransferencia <= saldo)
		         {
    		      printf ("\n Transferindo.......");
    		      printf ("\n Aguarde**************");
    	          printf ("\n *********************");
    	          sleep (tempo);
    	          printf("\7\7\7\7\7\7\7\7\7\7\7\n");//emite som
    		      printf("\n Transferencia de R$ %.2f, realizada com sucesso",valorTransferencia);
    		      saldo = (saldo - valorTransferencia);
    		      printf ("\n Seu saldo é R$ %.2f", saldo);
    		      //--------------------------------------------------------------------------
    		      printf ("\n ****************************************");
                  printf ("\n '1'(continuar) '2'(sair): ");
                  scanf("%d", &resp);
                  printf("\7\7\7\7\7\7\7\7\7\7\7\n");//emite som
                  system("clear");
                  //-------------------------------------------------------------------------------------
    		     }
		         if(valorTransferencia > saldo)
        		    {
        		       for(int i=0;i<=2;i++)
		                 {
		                  printf("\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\n");//emite som
		                  sleep(1);
		                 }
        		      printf ("\n Saldo insuficiente");
        		      printf("\n Transferencia de R$ %.2f, nao pode ser realizada",valorTransferencia);
        		      printf ("\n Seu saldo e de R$ %.2f", saldo);
        		      //--------------------------------------------------------------------------
        		      printf ("\n ****************************************");
                     printf ("\n '1'(continuar) '2'(sair): ");
                      scanf("%d", &resp);
                      printf("\7\7\7\7\7\7\7\7\7\7\7\n");//emite som
                      system("clear");
                      //------------------------------------------------------------------------
        		    }
                }
		    }
          if (z == 2)//menu transferencia CASO DESEJA CORRIGIR
    		{
    		  printf("\7\7\7\7\7\7\7\7\7\7\7\n");//emite som 
    		  system("clear");
    		  printf ("\n Informe Agencia");
    		  printf ("\n (Ex: 1234)");
    		  printf ("\n: ");
    		  scanf ("%d", &x);
    		  printf ("\n Informe a conta com digito");
    		  printf ("\n (EX: 123456)");
    		  printf ("\n: ");
    		  scanf ("%d", &y);
    		  printf ("\n Informe valor R$: ");
    		  scanf ("%f", &valorTransferencia);
    		  system("clear");
    		  printf("\7\7\7\7\7\7\7\7\7\7\7\n");//emite som
    		  printf ("\n Agencia_Conta");
    		  printf ("\n    %d_%d", x, y);
    		  printf ("\n R$ %.2f", valorTransferencia);
    		  printf("\7\7\7\7\7\7\7\7\7\7\7\n");//emite som
    		  system("clear");
    		  if (valorTransferencia <= saldo)
    		    {
    		      printf ("\n Transferindo.......");
    		      printf ("\n Aguarde**************");
    	          printf ("\n *********************");
    	          sleep (tempo);
    	          printf("\7\7\7\7\7\7\7\7\7\7\7\n");//emite som
    		      printf("\n Transferencia de R$ %.2f, realizada com sucesso",valorTransferencia);
    		      saldo = (saldo - valorTransferencia);
    		      printf ("\n Seu saldo C) R$ %.2f", saldo);
    		      //--------------------------------------------------------------------------
    		      printf ("\n ****************************************");
                  printf ("\n '1'(continuar) '2'(sair): ");
                  scanf("%d", &resp);
                  printf("\7\7\7\7\7\7\7\7\7\7\7\n");//emite som
                  system("clear");
                  //-------------------------------------------------------------------------------------
    		    }
		        else
		           if (valorTransferencia > saldo)
        		    {
        		      for(int i=0;i<=2;i++)
		                 {
		                  printf("\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\n");//emite som
		                  sleep(1);
		                 }
        		      system("clear");
        		      printf ("\n Saldo insuficiente");
        		      printf("\n Transferencia de R$ %.2f, nao pode ser realizada",valorTransferencia);
        		      printf ("\n Seu saldo e de R$ %.2f", saldo);
        		      //--------------------------------------------------------------------------
        		      printf ("\n ****************************************");
                      printf ("\n '1'(continuar) '2'(sair): ");
                      scanf("%d", &resp);
                      printf("\7\7\7\7\7\7\7\7\7\7\7\n");//emite som
                      system("clear");
                      //-------------------------------------------------------------------------------------
        		    }

		    }
		    if (opcao == 0)//menu sair
  
               {
                printf("\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\n");//emite som  
	            printf ("\n Obrigado, Volte sempre!");
	            system("clear");
	            return 0;
	           }
		     
	    }//fim de execulsao no laco (do)
      
        while(resp == 1);//opcao de sair apos realizar uma transacao
         {
            printf("\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\n");//emite som  
            printf ("\n Obrigado, Volte sempre!");
            return 0;
         }
    }

   
   
   else
   //se a senha for diferente de '0000'
	{
	  system("clear");
	  printf("\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7\7");
	  printf ("\n Senha incorreta");
	  
      return 0;
    }
}
