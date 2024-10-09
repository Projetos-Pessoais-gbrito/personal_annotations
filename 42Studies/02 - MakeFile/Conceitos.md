	É importante lembrar que o arquivo deve estar nomeado como 'Makefile'.
	Para criar todo arquivo Makefile teremos um alvo, uma dependencia e um comando, conforme abaixo:
```c
	Alvo (Arquivo alvo): Dependência (Arquivo ou variável)
		Comando	(Comando makefile)
		
```
###### Exemplo:
```c
	ft_puchar.c: main.c
			cc -Werror -Wall -Wextra main.c -o ft_putchar 
			
```
	O Makefile pode ter máscaras, são elas:
		$< # A primeira dependencia
		$@ # O alvo
		*.o # Qualquer .o
		%.o # Qualquer .o no alvo ou dependencia
