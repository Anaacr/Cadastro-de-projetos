# Cadastro de projetos
 Listagem de projetos, utilizando a linguagem C.


## Etapas do Programa
### Função main()
```c
int main(){
	setlocale(LC_ALL, "Portuguese");
	
	int escolha;
		
	do{
		system("cls");
		printf("**************************************************");
		printf("\n GESTÃO DE PROJETO ");
		printf("\n************************************************\n");
		printf("1 - Inserir projetos\n");
 		printf("2 - Listar todos os projetos\n");
 		printf("3 - Listar todos os projetos - A fazer\n");
 		printf("4 - Listar todos os projetos - Fazendo\n");
 		printf("5 - Listar todos os projetos - Concluído\n");
		printf("0 - Sair\n");
 		printf("Digite a opção desejada: ");
		scanf("%d", &escolha);
		
		switch(escolha){
			case 1:
				cadastrarProjetos();			
				break;
			case 2:
				listarProjetos();
				break;
			case 3:
				listarProjetosAfazer();
				break;
			case 4:
				listarProjetosFazendo();
				break;
			case 5:
				listarProjetosConcluido();
				break;
			default:
				printf("\nEscolha errada!!!\n");
				system("Pause");
		}
	}while(escolha != 0);
}
```
