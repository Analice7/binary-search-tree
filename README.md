# Árvore Binária de Busca (BST)

Este projeto implementa uma **Árvore Binária de Busca (BST)** em C, incluindo operações como inserção, remoção, busca, travessias e cálculo de altura.

## Estrutura da Árvore
A estrutura de um nó da BST está definida no arquivo `bst.h` e inclui:
- `valor`: o valor armazenado no nó;
- `esq`: ponteiro para o filho esquerdo;
- `dir`: ponteiro para o filho direito.

## Funções Implementadas

### Inserção
```c
arvore inserir (arvore raiz, int valor);
```
Insere um novo valor na BST, preservando suas propriedades.

### Travessias da Árvore
- **Pré-ordem**: `preorder(arvore raiz);`
- **Em ordem**: `inorder(arvore raiz);`
- **Pós-ordem**: `posorder(arvore raiz);`
- **Ordem reversa**: `reverso(arvore raiz);`

### Busca
```c
int buscar(arvore raiz, int valor);
```
Retorna `1` se o valor estiver na árvore e `0` caso contrário.

### Cálculo de Altura
```c
int altura(arvore raiz);
```
Retorna a altura da árvore (baseado no maior ramo).

### Contagem de Folhas
```c
void qtdFolhas(arvore raiz, int* total);
```
Calcula e armazena no ponteiro `total` o número de folhas da árvore.

### Impressão do Caminho até um Valor
```c
void caminho(arvore raiz, int valor);
```
Imprime o caminho da raiz até um determinado valor, se ele existir na árvore.

### Remoção
```c
arvore remover (arvore raiz, int valor);
```
Remove um valor da BST, ajustando a estrutura para manter suas propriedades.

### Busca pelo Maior Elemento
```c
arvore maiorElemento(arvore raiz);
```
Retorna o nó com o maior valor na subárvore informada.

## Como Compilar e Executar
1. Compile o código:
   ```sh
   gcc -o bst main.c bst.c
   ```
2. Execute o programa:
   ```sh
   ./bst
   ```

## Autor
Desenvolvido por Analice da Silva Nascimento.

