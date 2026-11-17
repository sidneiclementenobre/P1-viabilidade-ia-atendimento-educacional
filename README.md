# EduTriagem AI: Análise de Viabilidade, Riscos e Governança (PBL)

Estudo técnico-executivo desenvolvido para avaliar a viabilidade do uso de Inteligência Artificial (LLMs) na triagem, classificação e atendimento de mensagens estudantis em uma instituição de ensino digital.

## Pergunta Motriz
> *"Esse problema deveria realmente ser resolvido com inteligência artificial?"*

**Veredito:** **Não integralmente.** Recomenda-se uma **arquitetura híbrida** (regras determinísticas + IA como copiloto de triagem e rascunho + supervisão humana obrigatória), vetando decisões automatizadas em temas acadêmicos, financeiros ou disciplinares.

## Estrutura do Projeto (Níveis Incrementais)
* **Nível Básico:** Decomposição do problema, criação de dataset sintético com dados sensíveis e comparação de baseline (classificador por regras/palavras-chave vs. LLM).
* **Nível Intermediário:** Engenharia de prompts (comparação entre *prompt ingênuo* e *prompt estruturado* em JSON com baixa temperatura) e critérios de controle de alucinação.
* **Nível Avançado:** Análise de riscos éticos e legais (**LGPD**), implementação de camada local de anonimização (*PII Masking* via Regex), tratamento de falhas de disponibilidade (`Erro 503` / *fallback*) e matriz de governança.

## Como Executar no Google Colab
1. Abra o arquivo [P1_Viabilidade_IA_Atendimento_Educacional.ipynb](./P1_Viabilidade_IA_Atendimento_Educacional.ipynb) clicando no botão **"Open in Colab"** no topo do notebook.
2. Insira sua chave gratuita do Google AI Studio na variável `CHAVE_API` da primeira célula.
3. Execute as células sequencialmente.

