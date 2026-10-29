# Controle de fluxo em Java

Solução de um desafio da **Trilha Java Básico da DIO** para praticar entrada pelo terminal, laço `for` e exceções personalizadas.

## Como funciona

1. O programa solicita dois números inteiros.
2. Calcula a diferença entre o segundo e o primeiro.
3. Imprime uma sequência de 1 até o valor dessa diferença.
4. Se o primeiro número for maior que o segundo, lança `ParametrosInvalidosException` e exibe uma mensagem.

Exemplo de entrada:

```text
Primeiro parâmetro: 12
Segundo parâmetro: 15
```

Sequência impressa:

```text
Imprimindo o numero 1
Imprimindo o numero 2
Imprimindo o numero 3
```

## Como executar

Requer um JDK com `javac` e `java` disponíveis. Na raiz do repositório:

```sh
git clone https://github.com/JoaoAlencar00/desafioControleDeFluxo.git
cd desafioControleDeFluxo
mkdir build
javac -encoding UTF-8 -d build desafioControleFluxo/*.java
java -cp build desafioControleFluxo.Contador
```

## Estrutura

- `desafioControleFluxo/Contador.java`: leitura dos parâmetros, validação e contagem.
- `desafioControleFluxo/ParametrosInvalidosException.java`: exceção de negócio.

## Comportamentos atuais

Parâmetros iguais são aceitos e não geram impressões da sequência. O programa trata a ordem inválida dos números, mas não trata texto no lugar de números nem estouro na subtração de inteiros. Não há dependências externas ou testes automatizados no repositório.

## Créditos

Enunciado original da [DIO — Trilha Java Básico](https://www.dio.me/), de [Gleyson Sampaio](https://github.com/glysns). Este repositório registra a implementação do exercício.
