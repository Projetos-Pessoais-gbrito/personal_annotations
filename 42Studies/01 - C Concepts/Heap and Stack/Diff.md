- **`char* c = (char*)calloc(100, sizeof(char));`**:
    - Este código aloca um bloco de memória suficiente para armazenar 100 caracteres na heap. Inicialmente, todos os bytes são definidos como zero, permitindo que você armazene até 100 caracteres.
- **`char c[100];`**:
    - Aqui, você declara um array de 100 caracteres na stack. O array pode armazenar até 100 caracteres, mas não é inicializado automaticamente. Se você não o inicializar, ele pode conter valores aleatórios.- **`char* c = (char*)calloc(100, sizeof(char));`**:
    - Este código aloca um bloco de memória suficiente para armazenar 100 caracteres na heap. Inicialmente, todos os bytes são definidos como zero, permitindo que você armazene até 100 caracteres.