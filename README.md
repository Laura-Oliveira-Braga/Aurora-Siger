# Aurora-Siger - Relatório Operacional de Pré-Decolagem

## Descrição
Este repositório contém o projeto **Aurora Siger – Relatório Operacional de Pré-Decolagem**, desenvolvido como parte da Fase 1 da disciplina da FIAP. O trabalho integra conceitos de telemetria, algoritmos de verificação, automação em Python, análise energética, inteligência artificial e reflexão ética/sustentável. 

## Funcionalidades
- Organização e interpretação da telemetria inicial (temperatura, energia, pressão, integridade estrutural).  
- Algoritmo de verificação que decide entre **PRONTO PARA DECOLAR** ou **DECOLAGEM ABORTADA**.  
- Script em Python que automatiza as verificações.  
- Cálculo da autonomia energética considerando perdas.  
- Análise assistida por IA para identificar riscos.  
- Reflexão crítica sobre ética, impacto social e sustentabilidade.

## Estrutura do Repositório
- Relatório_PreDecolagem.pdf  # Documento final com todas as análises
- notebook.ipynb  # Código Python em formato jupyter notebook
- README.md  # Explicação do projeto com imagens/prints da execução

## Prints da Execução
**Telemetria Inicial:**
A telemetria deveria conter as seguintes informações: 
- Temperatura interna e externa;
- Integridade estrutural (0/1);
- Níveis de energia (%);
- Pressão dos tanques;
- Status dos módulos críticos.
Por não existirem dados reais de telemetria de espaçonaves para Marte, eu solicitei que a IA gerasse dados simulados em csv:
<img width="925" height="852" alt="dados de telemetria gerados por IA" src="https://github.com/user-attachments/assets/91402e2d-465a-4ef9-be50-e651db6c10d8" />

Após salvar estes dados em formato de CSV, eu os passei para o Google Collab e os organizei em uma tabela usando os comandos:
[import pandas as pd
dados = pd.read_csv('/content/dados_Aurora_Siger.csv', sep=',')
dados.head(10)]
<img width="1713" height="457" alt="Simulação de um Dataset" src="https://github.com/user-attachments/assets/c1a76db8-8509-4de5-a3a0-12e6accc41af" />
