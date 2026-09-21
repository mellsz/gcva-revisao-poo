# Atividade de Revisão — Orientação a Objetos

Atividade desenvolvida para a disciplina de **Gestão do Ciclo de Vida da Aplicação (GCVA)**, com o objetivo de revisar conceitos fundamentais de **Orientação a Objetos em Java**.

O projeto parte de um código simples de uma loja de consoles e realiza sua refatoração aplicando conceitos de POO e princípios de desenvolvimento trabalhados em aula.

## Conceitos aplicados

Durante a atividade foram trabalhados:

* Encapsulamento
* Construtores
* Interfaces
* Composição
* Herança
* Sobrescrita de métodos
* Polimorfismo
* Princípio de Substituição de Liskov (LSP)
* Princípio Aberto/Fechado (OCP)

## Estrutura do projeto

O sistema possui diferentes tipos de consoles:

* Nintendo
* Playstation
* Playstation Portátil
* Xbox

Todos os consoles seguem o contrato definido pela interface `IConsole`.

A classe `DadosConsole` é utilizada por composição para armazenar informações comuns, como nome e preço base.

A classe `PlaystationPortatil` herda de `Playstation` e sobrescreve seus comportamentos específicos.

A classe `Loja` trabalha apenas com objetos do tipo `IConsole`, permitindo que novos consoles sejam adicionados sem necessidade de alterar sua implementação.

## Funcionalidades

O programa permite:

* Ligar cada console;
* Calcular o preço final de acordo com o tipo de console;
* Realizar a venda de vários consoles;
* Calcular o faturamento total;
* Adicionar novos tipos de console mantendo a classe `Loja` inalterada.

## Percentuais utilizados

* Nintendo: 10%
* Playstation: 20%
* Playstation Portátil: 15%
* Xbox: 18%

## Execução

Para compilar:

```bash
javac Atividade_POO_Problema.java
```

Para executar:

```bash
java Atividade_POO_Problema
```

## Objetivo da atividade

O principal objetivo foi transformar um código baseado em atributos públicos e estruturas condicionais em uma solução orientada a objetos, distribuindo corretamente as responsabilidades entre as classes.

Com o uso de interfaces e polimorfismo, a classe `Loja` não precisa conhecer o tipo específico de cada console, permitindo que o sistema seja estendido com novos consoles sem modificar seu código.
