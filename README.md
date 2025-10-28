# azure-copilot-challenge-esg
# 🤖 Agente ESG: Calculadora de Empregabilidade Verde (Azure Frontier Girls Challenge)

![Azure](https://img.shields.io/badge/Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)

Este é o projeto de entrega para o "Build Your First Copilot Challenge" do programa Azure Frontier Girls, da Microsoft e WoMakersCode.

---

## 1. Descrição do Projeto e Objetivo do Agente
*(Requisito de Avaliação 4.a)*

### O Problema
Gestores públicos e organizações do terceiro setor precisam tomar decisões baseadas em dados para criar políticas de sustentabilidade e inclusão social. No entanto, estimar rapidamente o custo de programas de empregabilidade verde é um desafio que muitas vezes depende de planilhas complexas.

### O Objetivo do Agente (O Produto)
Este projeto é um **agente de IA (copiloto)** que atua como um "Assistente de Políticas Públicas ESG".

Seu objetivo é fornecer uma interface de conversação simples para que um gestor público possa estimar o custo de um programa de empregabilidade verde, bastando perguntar em linguagem natural.

## 2. Demonstração (A Ação Funcional)
*(Requisito de Avaliação 4.b - Prints de respostas, fluxo e execução)*

A "1 ação funcional" deste agente é um **cálculo** de custo. O agente usa uma "Tool" (ferramenta) de Python personalizada para executar a lógica de negócio.

### Exemplo de Interação (Print de Resposta)

Aqui você vai **colar um print (screenshot)** da interação com seu agente.

**Exemplo de Print:**
> **Usuário:** "Quanto custaria contratar 1.500 pessoas por 6 meses, com o salário mínimo de R$ 1.518,00?"
>
> **Agente ESG:** "O custo estimado para este programa seria de R$ 13.662.000,00. Este valor cobre o salário de 1.500 pessoas pelo período de 6 meses."

### Fluxo de Execução (A Arquitetura)

Este projeto utiliza um **orquestrador de IA** do framework da Microsoft para analisar a intenção do usuário e direcionar a tarefa para o agente correto.

**Diagrama do Fluxo:**
`[Usuário]` → `[Orquestrador (Azure)]` → `[Agente ESG]` → `[Tool: calcular_custo.py]` → `[Agente ESG]` → `[Usuário]`

*(Esta seção de arquitetura é o que mostra seu pensamento de "engenharia de produto" para o feedback da Motorola)*

## 3. Como Usar (Configuração do Projeto)

### Pré-requisitos
* Uma conta no Portal Azure
* Python 3.10+
* Git
* Azure CLI
* VS Code (recomendado)

### Passo a Passo da Configuração

1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/SEU_USUARIO/SEU_REPOSITORIO.git](https://github.com/SEU_USUARIO/SEU_REPOSITORIO.git)
    cd SEU_REPOSITORIO
    ```

2.  **Crie e ative o ambiente virtual:**
    ```bash
    python -m venv .venv
    .venv\Scripts\activate
    ```

3.  **Faça login no Azure (Obrigatório):**
    ```bash
    az login
    ```

4.  **Instale as dependências:**
    ```bash
    pip install -r requirements.txt
    ```
    *(**Importante:** Você deve criar um arquivo `requirements.txt` no seu repositório com o conteúdo: `openai`, `azure-ai-projects`, `azure-identity`, `agent-framework`, `python-dotenv`)*

5.  **Configure o arquivo `.env`:**
    Crie um arquivo `.env` e preencha com suas chaves do Azure OpenAI, conforme o notebook `criacao_agentes.ipynb`.

6.  **Execute o Notebook:**
    Abra o notebook principal do projeto no VS Code e execute as células.

## 4. Referências e Recursos
*(Requisito de Avaliação 4.c)*

* **Azure Frontier Girls (Repositório Base):** [Link para o repositório do programa da Microsoft]
* **Documentação do Azure AI Foundry:** [Link do Foundry]
* **Análise de Dados (TCC):** Este agente é baseado nos modelos de custo desenvolvidos no meu TCC do MBA em Data Science & Analytics (USP). O repositório completo da análise pode ser encontrado aqui: [Link para o seu repositório do TCC]

## 5. Autora

* **Amanda Morais** - [LinkedIn](https://www.linkedin.com/in/amandalearte)
