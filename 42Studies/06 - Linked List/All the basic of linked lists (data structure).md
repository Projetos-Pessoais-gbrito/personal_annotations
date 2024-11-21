<h1 align="center">Refer to this video here</h1>
	https://www.youtube.com/watch?v=N6dOwBde7-M&t=106s
<p>In Singly linked lists we have a node that knows just the next node and so on, the first node is gonna be known as the head node, with that we know what are the next adress, normally to implement linked list we have to analyse the situation, linked lists are good in inserting and reading non specified data in arrays of char.
To know that we are at the final of a linked list we have to know the null character, head to null pointer.</p>

![[Singly_linked_list.png]]

<p>To insert a element at the final of our linked list we have to iterate till the null pointer of the list and pass the final adress to the new nod and this new node will be pointed to null and the last will know its position.</p>
<h4 align="center">Observations</h4>

Se `new_node` for uma variável do tipo `Node` (não um ponteiro), você acessa seus campos usando o operador de ponto (`.`).
Exemplo:
```c
Node new_node; // Declara uma instância direta
new_node.data = 10; // Acessa diretamente o campo 'data'
new_node.next = NULL; // Acessa diretamente o campo 'next'
```

Se `new_node` for **um ponteiro para uma estrutura `Node`**, você acessa os campos da estrutura que o ponteiro está apontando usando o operador seta (`->`). 
Exemplo:
```C
Node* new_node = (Node*)malloc(sizeof(Node)); // Aloca memória para um 'Node'
new_node->data = 10; // Acessa o campo 'data' da estrutura apontada por 'new_node'
new_node->next = NULL; // Acessa o campo 'next' da estrutura apontada por 'new_node'
```

