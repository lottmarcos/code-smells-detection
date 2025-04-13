#  Avaliação de LLMs na Detecção de Code Smells e Recomendação de Refatorações

## Membros do Grupo

- Alan Augusto Martins Campos - 2021040121 (SI)
- Davi Esondem Menezes Brito - 2021039808 (SI)
- ⁠Fillipe de Oliveira Almeida - 2021040016 (SI)
- ⁠Marcos Lott de Araújo - 2021039786 (SI)

## Objetivo do Trabalho

Avaliar a capacidade de Modelos de Linguagem de Grande Escala (LLMs) em detectar code smells e recomendar refatorações, utilizando repositórios open-sources de projetos conhecidos por suas boas práticas de código. O objetivo é comparar as sugestões dos LLMs com ferramentas de análise estática de código (como o SonarQube) e manualmente, além de analisar qualitativamente os resultados.

## Metodologia
### Modelo de Linguagem que Será Usado

Para este trabalho utilizaremos o GPT-4, um modelo de linguagem de grande escala conhecido por suas capacidades avançadas de compreensão e geração de texto. O GPT-4 será utilizado para identificar code smells e sugerir refatorações nos trechos de código fornecidos.

### Datasets
Selecionamos um conjunto de repositórios de código aberto conhecidos por suas boas práticas de desenvolvimento e qualidade de código. Os repositórios escolhidos incluem:

- **Spring Framework**: Um dos mais populares frameworks para desenvolvimento de aplicações Java.
- **Django**: Um framework web de alto nível para Python, que incentiva o desenvolvimento rápido e o design limpo e pragmático.

Esses repositórios foram selecionados por sua ampla adoção, documentação robusta e histórico de manutenção ativa.

### Exemplos Preliminares de Prompts

Para interagir com o GPT-4, utilizaremos os seguintes exemplos de prompts:

#### Detecção de Code Smells:
```
"Identifique se há ou não algum code smell neste código. No caso positivo, explique por que ele é problemático"
```
```
"Sugira uma refatoração que resolva esse code smell."
```
## Avaliação Quantitativa

A avaliação quantitativa será realizada comparando as sugestões de code smells e refatorações fornecidas pelo GPT-4 com as identificadas pela ferramenta de análise estática de código SonarQube. As métricas utilizadas incluirão:

- **Acurácia:** A proporção entre o total de acertos da LLM em relação ao total de amostras fornecidas
- **Precisão:** A proporção de code smells identificados corretamente pelo LLM em relação ao total de code smells identificados.
- **Recall:** A proporção de code smells identificados pelo LLM em relação ao total de code smells existentes.

## Avaliação Qualitativa

A avaliação qualitativa envolverá uma análise manual de um conjunto selecionado de exemplos para identificar padrões de sucesso e áreas de melhoria. Esta análise incluirá:

- **Exemplos Eficazes:** Casos onde o LLM identificou corretamente os code smells e sugeriu refatorações apropriadas.
- **Exemplos Ineficazes:** Casos onde o LLM falhou em identificar code smells ou sugeriu refatorações insuficientes.

Os resultados qualitativos serão documentados com explicações detalhadas sobre a eficácia das sugestões do LLM em comparação com as ferramentas tradicionais de análise de código.

