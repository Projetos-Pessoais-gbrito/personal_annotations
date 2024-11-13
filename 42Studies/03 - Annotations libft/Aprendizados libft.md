#### **Função memmove**

Copia uma array de char 'src' para um array de char 'dst', ela checa antes de copiar se terá uma sobreposição de conteudos caso dst esteja dentro de src.
O exemplo abaixo mostra que dst está 'dentro' de src e nós queremos copiar 5 caracteres de src para dst, nesse caso teriamos uma sobreposição pois a primeira letra src ficaria por cima de W que é o local que dst está localizado.

Memória:    | 0x00 | 0x01 | 0x02 | 0x03 | 0x04 | 0x05 | 0x06 | 0x07 | 0x08 | 0x09 |
Conteúdo:   |  H       |  e     |  l         |  l       |  o       |  ,        |  W      |  o      |  r        |  l        |
Endereços:  | src     |         |            |          |           |           | dest   |          |            |          |


*void *memmove(*void* dest, *const *void* src, *size_t n)

Acima é como a função memmove é instanciada, ela retorna qualquer tipo de dado pois seu retorno é void* que indica que pode ser um ponteiro para qualquer tipo.

Ex ft_strlcpy:
- Truncamento significa que houve um corte de alguma parte do conteudo que voce está utilizando.
