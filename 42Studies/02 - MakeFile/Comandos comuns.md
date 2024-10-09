### Principais comandos
	- Para fazer uma execução silenciosa basta colocar um "@"
```c 
	@echo "Olá Mundo"

	Execução no terminal
		"Olá Mundo"
```
	- É possível definir variaveis dentro do MakeFile, conforme exemplo abaixo.
```c 
	@echo "Olá Mundo"

	Execução no terminal
		"Olá Mundo"
```
	-Make clean
	Caso o arquivo esteja dentro de uma pasta especifica é necessário especifica-la, pastaEspecifica/*.o
```c 
	clean:
		rm *.o
```
	É possível definir variaveis dentro de um make file, conforme exemplo abaixo:
```c 
	PRINCIPAL_DIRETORIO:./caminho_especifico
```
	Dessa forma acima basta apenas reutilizar esse caminho acima em outras partes do Makefile.
	- EX_DIRS := $(wildcard cExercices/ex*/) define a variavel por todos que arquivos que comecam com ex e tem um valor indefinido.