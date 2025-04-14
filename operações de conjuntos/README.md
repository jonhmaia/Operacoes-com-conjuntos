# 🔢 Projeto de Operações com Conjuntos em C

Este projeto implementa uma biblioteca em C para manipulação de **conjuntos de números inteiros longos** (`long int`), com suporte a diversas operações fundamentais da teoria de conjuntos. É possível criar conjuntos, inserir e remover elementos, realizar interseções, uniões, verificar subconjuntos, entre outros.

---

## 📦 Estrutura

- `conjuntos.h`: Definição da estrutura `Conjunto` e declaração das funções.
- `conjuntos.c`: Implementação das funções de manipulação de conjuntos.
- `main.c`: Interface de terminal interativa para testar as funcionalidades.
- `README.md`: Documentação do projeto.

---

## ⚙️ Funcionalidades implementadas

- ✅ Criação e destruição de conjuntos
- ✅ Inserção e remoção de elementos
- ✅ Verificação se o conjunto está vazio
- ✅ Cálculo da cardinalidade (quantidade de elementos)
- ✅ Impressão de conjuntos
- ✅ Ordenação crescente/decrescente
- ✅ Verificação de pertencimento de elementos
- ✅ Cálculo do maior e menor elemento
- ✅ Contagem de elementos maiores ou menores que um valor
- ✅ Verificação de igualdade entre conjuntos
- ✅ Verificação de subconjunto
- ✅ Cálculo do conjunto complemento
- ✅ Cálculo da união e interseção entre conjuntos
- ✅ Cópia entre conjuntos

---

## 🚀 Como compilar e executar

### ✅ Pré-requisitos

- Ter um compilador C instalado (como `gcc`)
- Sistema operacional compatível com terminal (Linux, macOS ou Windows com WSL/MinGW)

### 🧪 Compilação simples com `gcc`

Abra o terminal na pasta do projeto e execute:

```bash
gcc main.c conjuntos.c -o conjuntos
```

Se o comando não gerar erros, o executável `conjuntos` será criado.

### ▶️ Execução do programa

Após a compilação, execute o programa com:

```bash
./conjuntos
```

Se estiver no Windows, use:

```bash
conjuntos.exe
```

---

### 🔁 (Opcional) Usando Makefile

Você pode criar um arquivo chamado `Makefile` com o seguinte conteúdo:

```makefile
all:
	gcc main.c conjuntos.c -o conjuntos

run: all
	./conjuntos
```

Depois, é só usar:

```bash
make run
```

---

### ❗ Dicas úteis

- Se o terminal retornar erro como "gcc: command not found", instale o GCC com:
  - Ubuntu/Debian: `sudo apt install build-essential`
  - macOS: `xcode-select --install`
  - Windows: instale o [MinGW](http://www.mingw.org/)

- Certifique-se de que todos os arquivos `main.c`, `conjuntos.c` e `conjuntos.h` estão no mesmo diretório

---

## 🧪 Exemplo de uso

```c
Conjunto *A = cria_conjunto();
insere_elemento(A, 10);
insere_elemento(A, 20);
print_conjunto(A); // Deve imprimir: 10 20
```

No terminal, o programa pedirá:

```bash
Quantos conjuntos deseja criar?
# => 2

Qual operação deseja realizar?
# => Selecione uma opção entre as listadas no menu
```

---

## 📌 Observações

- Cada conjunto pode conter até **10 elementos únicos**.
- O código inclui mensagens coloridas para facilitar a leitura das respostas no terminal.
- Operações como união, interseção e complemento respeitam os limites da cardinalidade máxima.

---

## 👩‍💻 Autoria

Desenvolvido por **João Marcos Araújo Maia**  
Estudante de Ciência da Computação - UFG  
Estagiária em Software Engineering na BigDataCorp  
🔗 [LinkedIn](https://www.linkedin.com/in/joaomarcosmaia) | 🌐 [Portfólio](https://joaomarcos.dev.br)

---

## 📄 Licença

Este projeto está licenciado sob a [MIT License](https://opensource.org/licenses/MIT).
