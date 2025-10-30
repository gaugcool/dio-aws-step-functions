# Desafio DIO – AWS Step Functions (Hello World)

## Descrição do Projeto
Este projeto foi desenvolvido como parte do **desafio da DIO** para praticar e consolidar conhecimentos sobre o **AWS Step Functions**, um serviço de orquestração de workflows na AWS.  
O objetivo principal foi criar um **Hello World State Machine** para entender como funcionam os estados, transições e execução de fluxos automatizados.

---

## Objetivos de Aprendizagem
- Aplicar conceitos do AWS Step Functions em um ambiente prático.  
- Criar e executar uma State Machine com sucesso.  
- Documentar o processo de forma clara para estudo e compartilhamento.

---

## Workflow Criado

O workflow criado é baseado no **Hello World Example** fornecido pela AWS. Ele contém os seguintes estados:

| Estado                     | Tipo     | Função                                                       |
|-----------------------------|----------|-------------------------------------------------------------|
| Set Variables and State Output | Pass    | Cria variáveis iniciais e define parâmetros do fluxo.      |
| Is Hello World Example?     | Choice   | Decide se o fluxo é realmente um exemplo Hello World.      |
| Wait for X Seconds          | Wait     | Aguarda 3 segundos antes de continuar a execução.          |
| Execute in Parallel         | Parallel | Executa duas ações em paralelo: formata a data e calcula o tempo decorrido. |
| Set Checkpoint              | Pass     | Atualiza a contagem de checkpoints do fluxo.               |
| Summarize the Execution    | Succeed  | Finaliza a execução com sucesso e gera um resumo no output.|

---

## Execução da State Machine

1. Acesse o console **AWS Step Functions**.  
2. Selecione a máquina de estado criada: `HelloWorld

  "Summary": "This Hello World execution began on 10/30. The state machine ran for 3 seconds before the snapshot was taken, passing through 2 checkpoints, and has successfully completed."
}
