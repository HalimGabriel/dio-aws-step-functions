# AWS Step Functions - Criando Workflows Automatizados | DIO

Repositório desenvolvido para o desafio da **Formação AWS Cloud Foundations** da **Digital Innovation One (DIO)**, com o objetivo de documentar os conceitos e a prática de criação de workflows automatizados utilizando o **AWS Step Functions**.

## O que é o AWS Step Functions?

O **AWS Step Functions** é um serviço de orquestração da AWS que permite criar fluxos de trabalho (workflows) compostos por diferentes etapas. Esses fluxos são definidos por **State Machines**, que coordenam serviços da AWS, funções Lambda e outras tarefas de forma visual, escalável e sem a necessidade de gerenciar servidores.

## Conceitos aprendidos

### State Machine

É a estrutura principal do AWS Step Functions. Ela define o fluxo de execução, os estados que compõem o processo e as transições entre cada etapa.

### Estados (States)

Durante o laboratório foram utilizados e estudados os principais tipos de estados:

* **Pass:** encaminha dados para o próximo estado sem realizar processamento.
* **Wait:** pausa a execução do workflow por um período definido.
* **Task:** executa uma tarefa, como chamar uma função AWS Lambda.
* **Choice:** cria decisões condicionais dentro do fluxo.
* **Succeed:** encerra o workflow com sucesso.
* **Fail:** encerra o workflow indicando falha.

## Workflow criado no laboratório

O workflow desenvolvido possui uma estrutura simples para demonstrar o funcionamento das State Machines.

Fluxo da execução:

1. **MensagemInicial** – Estado `Pass` que cria uma mensagem de saída.
2. **Esperar** – Estado `Wait` que pausa a execução por alguns segundos.
3. **Finalizado** – Estado `Succeed` que finaliza o workflow com sucesso.

Esse fluxo demonstra a criação, execução e conclusão de uma State Machine utilizando apenas recursos do AWS Step Functions.

## Benefícios do AWS Step Functions

* Automatização de processos.
* Orquestração de múltiplos serviços da AWS.
* Execução de workflows serverless.
* Tratamento de erros com mecanismos de Retry e Catch.
* Monitoramento completo do histórico de execução.
* Escalabilidade automática.

## Casos de uso

* Processamento de pedidos.
* Pipelines de ETL e processamento de dados.
* Aprovação de documentos.
* Automação de processos entre serviços AWS.
* Orquestração de aplicações serverless.

## Execução do laboratório

Durante a prática foram realizadas as seguintes etapas:

* Criação de uma State Machine do zero.
* Configuração de um workflow no editor do Step Functions.
* Execução da State Machine pelo console da AWS.
* Visualização do diagrama de execução.
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

## Capturas de tela

### Tela inicial do AWS Step Functions

> Inserir imagem em `images/home-step-functions.png`.

### Criação da State Machine

> Inserir imagem em `images/create-state-machine.png`.

### Editor do Workflow

> Inserir imagem em `images/workflow-editor.png`.

### Diagrama da State Machine

> Inserir imagem em `images/workflow-diagram.png`.

### Execução concluída

> Inserir imagem em `images/execution-success.png`.

### Histórico da execução

> Inserir imagem em `images/execution-history.png`.

## Tecnologias utilizadas

* AWS Step Functions
* Git
* GitHub
* Markdown

## Aprendizados

Este desafio permitiu compreender como o AWS Step Functions organiza processos automatizados por meio de máquinas de estado, facilitando a criação de workflows escaláveis, monitoráveis e integrados com outros serviços da AWS. Além disso, foi possível acompanhar toda a execução do fluxo pelo console da AWS e entender como cada estado participa do processo.

## Conclusão

O AWS Step Functions é uma ferramenta essencial para orquestração de aplicações serverless e automação de processos na nuvem. Com ele é possível construir workflows claros, reutilizáveis e fáceis de monitorar, reduzindo a complexidade de integrações entre diferentes serviços da AWS.
