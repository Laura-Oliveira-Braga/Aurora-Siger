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
**1.1 Telemetria Inicial:**
A telemetria deve conter as seguintes informações: 
- Temperatura interna e externa;
- Integridade estrutural (0/1);
- Níveis de energia (%);
- Pressão dos tanques;
- Status dos módulos críticos.

Por não existirem dados reais de telemetria de espaçonaves para Marte, eu solicitei que a IA gerasse dados simulados em csv:

<img width="925" height="852" alt="dados de telemetria gerados por IA" src="https://github.com/user-attachments/assets/91402e2d-465a-4ef9-be50-e651db6c10d8" />

Após salvar estes dados em formato de CSV, eu fiz o upload para o Google Collab e os organizei em uma tabela usando os comandos:

[import pandas as pd],
[dados = pd.read_csv('/content/dados_Aurora_Siger.csv', sep=',')] e
[dados.head(10)]

<img width="1713" height="457" alt="Simulação de um Dataset" src="https://github.com/user-attachments/assets/c1a76db8-8509-4de5-a3a0-12e6accc41af" />


**1.2 Algoritmo de Verificação:**
Cria-se uma lógica simples que decide: 
- Se todos os valores estão dentro da faixa segura → PRONTO PARA DECOLAR;
- Se algum valor está fora → DECOLAGEM ABORTADA.

Eu criei este algoritmo por meio de pseudocódigo:

<img width="741" height="676" alt="Algoritmo de verificação" src="https://github.com/user-attachments/assets/4a832a58-5db2-4e47-84ec-15d4a99efd86" />


**1.3 Script em Python:**
Trasnformar o pseudocódigo em código real: 
- Simulando a leitura dos dados;
- Execução das verificações;
- Resultado final impresso.

<img width="837" height="730" alt="Script em Python" src="https://github.com/user-attachments/assets/35c9f4ff-45db-4db3-9201-b38594450c04" />


**1.4 Análise energética**
A partir dos dados apresentados, calcular autonomia inicial considerando:
- Capacidade total (kwh);
- Carga atual (%);
- Consumo estimado na decolagem;
- Perdas energéticas.

Para realizar tais cálculos, usasse as seguintes fórmulas:
1. Energia disponível = Capacidade total (KWh) * Carga atual (%) / 100
2. Energia líquida após perdas = Energial disponível - Perdas energéticas (KWh)
3. Autonomia incial = Energia líquida - Consumo estimado na decolagem (KWh)

Em Python:

<img width="993" height="593" alt="Análise energética" src="https://github.com/user-attachments/assets/710fcb15-d39f-4b45-991e-f61101dbb159" />


**1.5 Análise assistida por IA**
Usando a assitintência de IA do próprio Google Collaboratory, eu solicitei qu o Gemini:
- Classificasse os dados;
- Identificasse possíveis anomalias;
- Desse sugestões de risco.

O resultado de sua análise foi:

<img width="1396" height="557" alt="Analise de dados por IA" src="https://github.com/user-attachments/assets/25e92fa5-541b-41b9-8a85-d48dc41515b8" />

Sua resposta dentro do python:

<img width="1061" height="737" alt="Análise assistida por IA" src="https://github.com/user-attachments/assets/f9033332-171b-4bb8-b040-896d9dba45be" />


**1.6 Refexão Crítica**
A exploração espacial exige uma postura ética rigorosa, é essencial garantir que cada decisão respeite a vida humana, os recursos naturais e o futuro das próximas gerações, inclui transparência, segurança e uso consciente dos investimentos, também envolve evitar a militarização do espaço e assegurar que o conhecimento adquirido seja compartilhado para benefício coletivo.

Missões espaciais inspiram novas gerações, estimulam avanços científicos e tecnológicos e criam empregos, ao mesmo tempo, levantam questões sobre desigualdade, se apenas grandes potências ou corporações dominarem esse campo, o risco é ampliar disparidades globais, por outro lado, pode gerar inclusão, educação e até soluções.

A construção de espaçonaves, o uso de combustíveis e a geração de resíduos espaciais precisam ser pensados para não comprometer o equilíbrio do planeta e do próprio espaço. Tecnologias sustentáveis, como sistemas de reciclagem de recursos, energia solar avançada e design modular, são fundamentais para reduzir impactos. A ideia é que a exploração espacial não seja uma fuga da Terra, mas um laboratório para desenvolver soluções que ajudem a preservar nosso planeta.

Só faz sentido avançar rumo a Marte e além se houver compromisso ético, impacto social inclusivo e tecnologias sustentáveis.

## Resultados
1. Telemetria organizada e interpretada.
2. Algoritmo funcional em Python.
3. Autonomia energética calculada.
4. Reflexão crítica sobre ética e sustentabilidade.

## Autor
Projeto desenvolvido por Laura Oliveira Braga, estudante do 1° semestre da FIAP, como parte da Fase 1 da missão Aurora Siger.
