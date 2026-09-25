# AWS Step Functions - Criando Workflows Automatizados | DIO

Repositório desenvolvido para o desafio da **Formação AWS Cloud Foundations** da **Digital Innovation One (DIO)**, com o objetivo de documentar os conceitos e a prática de criação de workflows automatizados utilizando o **AWS Step Functions**.

## O que é o AWS Step Functions?

O **AWS Step Functions** é um serviço de orquestração da AWS que permite criar fluxos de trabalho (workflows) compostos por diferentes etapas. Esses fluxos são definidos por **State Machines**, que organizam as etapas e transições de um processo de forma visual e escalável.

## Conceitos aprendidos

### State Machine

É a estrutura principal do AWS Step Functions. Ela define o fluxo de execução, os estados que compõem o processo e as transições entre cada etapa.

### Estados (States)

O AWS Step Functions possui diferentes tipos de estados que podem ser utilizados para construir workflows.

Durante este laboratório, foram utilizados:

* **Pass:** encaminha dados para o próximo estado sem realizar processamento.
* **Wait:** pausa a execução do workflow por um período definido.
* **Succeed:** encerra o workflow com sucesso.

Outros tipos de estados disponíveis incluem:

* **Task:** executa uma tarefa, podendo realizar integrações com outros serviços da AWS.
* **Choice:** permite criar decisões condicionais dentro do fluxo.
* **Fail:** encerra o workflow indicando uma falha.

## Workflow criado no laboratório

O workflow desenvolvido possui uma estrutura simples para demonstrar o funcionamento de uma State Machine.

### Fluxo da execução

1. **MensagemInicial** – Estado `Pass` que cria uma mensagem de saída.
2. **Esperar** – Estado `Wait` que pausa a execução por alguns segundos.
3. **Finalizado** – Estado `Succeed` que finaliza o workflow com sucesso.

Esse fluxo demonstra a criação, execução e conclusão de uma State Machine utilizando o AWS Step Functions.

## Benefícios do AWS Step Functions

* Automatização de processos.
* Orquestração de diferentes etapas de um workflow.
* Criação de processos serverless.
* Tratamento de erros e controle de fluxo.
* Acompanhamento das execuções.
* Visualização do histórico de eventos.

## Casos de uso

O AWS Step Functions pode ser utilizado em diferentes cenários, como:

* Processamento de pedidos.
* Pipelines de ETL e processamento de dados.
* Aprovação de documentos.
* Automação de processos entre serviços AWS.
* Orquestração de aplicações serverless.

## Execução do laboratório

Durante a prática foram realizadas as seguintes etapas:

* Criação de uma State Machine do zero.
* Configuração de um workflow utilizando o editor do Step Functions.
* Definição dos estados `Pass`, `Wait` e `Succeed`.
* Execução da State Machine pelo console da AWS.
* Visualização do diagrama do workflow.
* Acompanhamento da execução.
* Consulta ao histórico de eventos da execução.

## Estrutura do repositório

```text
📦 dio-aws-step-functions
 ┣ 📂 images
 ┃ ┣ home-step-functions.png
 ┃ ┣ create-state-machine.png
 ┃ ┣ workflow-editor.png
 ┃ ┣ workflow-diagram.png
 ┃ ┣ execution-success.png
 ┃ ┗ execution-history.png
 ┗ 📄 README.md
```

## Tecnologias utilizadas

* AWS Step Functions
* Git
* GitHub
* Markdown

## Aprendizados

Este desafio permitiu compreender como o AWS Step Functions organiza processos automatizados por meio de máquinas de estado. Durante a prática, foi possível criar uma State Machine, configurar diferentes estados, executar o workflow e acompanhar cada etapa de sua execução pelo console da AWS.

Também foi possível compreender como os estados podem ser utilizados para controlar o fluxo de um processo e como o histórico de eventos permite acompanhar o comportamento da execução.

## Conclusão

O AWS Step Functions permite criar e gerenciar workflows compostos por diferentes etapas, facilitando a organização e a automação de processos na AWS.

A prática realizada neste laboratório proporcionou uma introdução à criação de State Machines, configuração de estados, execução de workflows e acompanhamento dos resultados através do console da AWS.
