# YPO — Prompts de Teste para Ferramentas Agênticas

> Cada prompt abaixo está pronto para ser colado diretamente na ferramenta sendo testada.
> Os documentos de apoio estão nas subpastas por Task.
> Teste um de cada vez e registre os resultados na tabela de entregáveis.

---

## TASK 1.1 — Resposta de Business Development
**Nível:** 1 | **Dificuldade:** Baixa | **Documentos necessários:** `1.1_email_parceiro.md`, `1.1_tese_de_investimento.md`

---

### PROMPT

```
Você é o assistente executivo do CEO da Vértice Capital & Tecnologia.

Acabei de receber o e-mail e o deck resumido da empresa LogiSul Soluções Ltda (arquivo: 1.1_email_parceiro.md), que está propondo uma parceria comercial.

Leia atentamente o e-mail e o deck da LogiSul. Em seguida, leia nossa tese de investimento e diretrizes estratégicas (arquivo: 1.1_tese_de_investimento.md).

Com base nesses dois documentos, gere exatamente 3 opções de resposta de e-mail, identificadas como Opção A, Opção B e Opção C:

- **Opção A — Recusa Educada:** Decline a parceria de forma respeitosa e profissional, sem fechar portas definitivamente. Mencione pelo menos um motivo específico alinhado com nossa tese de investimento.

- **Opção B — Pedido de Mais Informações:** Demonstre interesse moderado e solicite dados específicos que faltam para uma avaliação adequada. Liste de 3 a 5 perguntas concretas baseadas nos gaps que você identificou no deck da LogiSul.

- **Opção C — Aceite com Agenda Sugerida:** Aceite uma reunião de apresentação e proponha uma agenda de 45 minutos com tópicos específicos que queremos abordar, alinhados com nossa estratégia.

Formato de cada opção:
- Assunto do e-mail
- Corpo completo do e-mail (tom formal, em português, assinado pelo CEO)
- [Nota interna: justificativa em 2 linhas de por que esta opção é adequada]

Ao final, indique qual das 3 opções você recomenda e por quê.
```

---

## TASK 1.2 — Curadoria de Networking (LinkedIn Export)
**Nível:** 1 | **Dificuldade:** Baixa/Média | **Documentos necessários:** `1.2_linkedin_export.csv`

---

### PROMPT

```
Você é um analista estratégico de relacionamentos executivos.

Tenho aqui o export das minhas conexões do LinkedIn (arquivo: 1.2_linkedin_export.csv). Preciso que você realize as seguintes ações:

**Etapa 1 — Classificação Setorial**
Leia todos os contatos e classifique cada um nas seguintes categorias de setor:
- Tecnologia & SaaS
- Agronegócio & Commodities
- Serviços Financeiros & Fintechs
- Logística & Infraestrutura
- Saúde & Farma
- Varejo & Consumer
- Outros

Apresente uma tabela com: Nome | Empresa | Cargo | Setor Classificado

**Etapa 2 — Identificação de Power Players**
Dos contatos classificados, identifique os "Power Players": pessoas que ocupam cargos de CEO, COO, CFO, CTO, Diretor, VP, Sócio ou Fundador em empresas com presença relevante no mercado (S/A, multinacionais ou startups com mais de 50 funcionários visíveis no perfil/empresa).

Liste os Power Players em uma tabela separada com: Nome | Cargo | Empresa | Por que é um Power Player

**Etapa 3 — Mensagens de Re-aproximação**
Para cada Power Player identificado, redija uma mensagem personalizada de re-aproximação (máximo 5 linhas) para envio direto pelo LinkedIn. A mensagem deve:
- Referenciar a empresa ou setor de atuação do contato (algo específico, não genérico)
- Ter tom natural e executivo, sem parecer spam
- Propor um próximo passo claro (call, café, troca de insights)
- Ser diferente para cada contato (sem copiar e colar o mesmo template)

Apresente as mensagens no formato: **[Nome]** → [Mensagem]

Ao final, apresente um resumo: total de contatos, distribuição por setor (%), quantidade de Power Players identificados.
```

---

## TASK 2.1 — Pipeline de Triagem M&A / Fornecedores
**Nível:** 2 | **Dificuldade:** Média | **Documentos necessários:** `2.1_empresas_alvo.md`

---

### PROMPT

```
Você é um analista de M&A sênior trabalhando para um grupo de investimentos brasileiro.

Recebi uma lista de 5 empresas que estamos avaliando como alvos de aquisição ou parceria estratégica (arquivo: 2.1_empresas_alvo.md). Preciso de uma análise rápida para apresentar ao comitê de investimentos ainda esta semana.

Execute as seguintes etapas para **cada uma das 5 empresas**, na ordem:

**Etapa 1 — Pesquisa de Notícias Recentes**
Acesse a internet e busque notícias dos últimos 12 meses sobre cada empresa. Foque em: movimentações estratégicas, captações/rodadas de investimento, expansões, demissões em massa, problemas regulatórios, mudanças de liderança ou qualquer evento relevante. Cite a fonte e a data de cada notícia encontrada.

**Etapa 2 — Modelo de Receita**
Com base no site da empresa e nas notícias encontradas, descreva o provável modelo de receita: como a empresa ganha dinheiro, quais seus principais produtos/serviços, estimativa de ticket médio, perfil de cliente e se é recorrente (SaaS/assinatura) ou transacional.

**Etapa 3 — Análise SWOT**
Gere uma análise SWOT completa com pelo menos 3 pontos em cada quadrante (Forças, Fraquezas, Oportunidades, Ameaças). Os pontos devem ser específicos e fundamentados nas informações coletadas — não genéricos.

**Entrega Final**
Após analisar as 5 empresas individualmente, gere:
1. Uma tabela comparativa SWOT com as 5 empresas lado a lado
2. Um ranking das empresas por atratividade para aquisição (1 = mais atraente), com 3 linhas de justificativa para cada posição
3. Recomendação final: qual empresa priorizar para due diligence e por quê

Formato da tabela comparativa:
| Critério | Empresa 1 | Empresa 2 | Empresa 3 | Empresa 4 | Empresa 5 |
(uma linha por ponto de SWOT)
```

---

## TASK 2.2 — Assistente de Onboarding de Clientes e Contratos
**Nível:** 2 | **Dificuldade:** Média | **Documentos necessários:** `2.2_minuta_contrato_template.docx`, `2.2_dados_cliente.md`, `2.2_guia_clausulas_risco.md`

---

### PROMPT

```
Você é o assistente jurídico-operacional responsável pelo onboarding de novos clientes.

Tenho os seguintes documentos:
- Minuta padrão de contrato de prestação de serviços (arquivo: 2.2_minuta_contrato_template.docx)
- Dados brutos do novo cliente (arquivo: 2.2_dados_cliente.md)
- Guia de cláusulas de risco da empresa (arquivo: 2.2_guia_clausulas_risco.md)

Execute as 3 etapas abaixo:

**Etapa 1 — Preenchimento da Minuta**
Substitua todos os campos placeholder da minuta ([NOME_CLIENTE], [CNPJ], [OBJETO], [VALOR], [PRAZO], [DATA_INICIO], etc.) pelos dados do cliente fornecidos. Apresente o contrato preenchido na íntegra, mantendo toda a formatação e numeração de cláusulas originais.

**Etapa 2 — Identificação de Cláusulas de Risco**
Com base no guia de cláusulas de risco (arquivo: 2.2_guia_clausulas_risco.md), analise o contrato preenchido e identifique:
- Cláusulas que apresentam risco jurídico ou operacional para nossa empresa
- Campos que ficaram em branco ou ambíguos
- Qualquer inconsistência entre os dados do cliente e os termos do contrato

Apresente cada risco no formato:
> **[Cláusula X.X]** — Risco: [descrição] | Recomendação: [ação sugerida]

**Etapa 3 — E-mail para o Jurídico**
Redija um e-mail profissional para o departamento jurídico (destinatário: juridico@vertice.com.br) com:
- Assunto claro identificando o cliente e o tipo de contrato
- Resumo do contrato (objeto, valor, prazo) em 3 linhas
- Lista dos riscos identificados na Etapa 2
- Solicitação explícita de revisão antes da assinatura
- Prazo sugerido para retorno (use 3 dias úteis a partir de hoje)

Tom: formal e objetivo. O e-mail deve ser enviável sem edição adicional.
```

---

## TASK 3.1 — Transformação de Relatório de RI em Deck de Board
**Nível:** 3 | **Dificuldade:** Alta | **Documentos necessários:** `3.1_relatorio_trimestral.md`, `3.1_noticias_setor.md`

---

### PROMPT

```
Você é um consultor estratégico especializado em Relações com Investidores e comunicação para Board.

Recebi o relatório trimestral da Vértice Agro S/A (arquivo: 3.1_relatorio_trimestral.md) e uma coletânea de notícias do setor do mesmo período (arquivo: 3.1_noticias_setor.md). Preciso transformar isso em um roteiro de apresentação para o Board de Diretores.

Execute as 3 etapas abaixo:

**Etapa 1 — Extração dos 5 KPIs Principais**
Leia o relatório trimestral e extraia os 5 KPIs financeiros mais relevantes para o Board. Para cada KPI, informe:
- Nome do indicador
- Valor atual (trimestre)
- Comparativo: variação vs. trimestre anterior e vs. mesmo período do ano anterior (%)
- Tendência: positiva, negativa ou estável
- Fonte exata no relatório (página/seção)

**Etapa 2 — Análise de Sentimento do Mercado**
Leia as notícias do setor (arquivo: 3.1_noticias_setor.md) e identifique:
- O sentimento geral do mercado no período: otimista, neutro ou pessimista
- Os 3 principais temas/eventos que estão influenciando o setor
- Como esses fatores externos se relacionam com os resultados da Vértice Agro (positivamente ou negativamente)
- Riscos e oportunidades do cenário externo para os próximos 2 trimestres

**Etapa 3 — Roteiro da Apresentação (10 Slides)**
Estruture o roteiro completo de uma apresentação de 10 slides para o Board. Para cada slide, especifique:

> **Slide [N] — [Título]**
> Objetivo: [o que este slide precisa comunicar]
> Conteúdo principal: [bullet points do que mostrar]
> Tipo de visualização recomendado: [ex: gráfico de barras, linha do tempo, tabela comparativa, mapa de calor, texto com ícones]
> Mensagem-chave: [a única frase que o Board deve lembrar deste slide]

A narrativa deve seguir a estrutura: Contexto → Resultados → Análise Externa → Riscos → Próximos Passos.

Ao final, escreva um parágrafo de "Abertura do CEO" (máximo 5 linhas) para ser lido no início da apresentação, sintetizando o trimestre em tom executivo.
```

---

## TASK 3.2 — Auditoria de Processo e Identificação de Gargalos
**Nível:** 3 | **Dificuldade:** Alta | **Documentos necessários:** `3.2_workflow_atual.md`

---

### PROMPT

```
Você é um consultor especialista em automação de processos e implementação de IA em empresas B2B.

Recebi a descrição detalhada do processo atual de vendas e entrega de software da nossa empresa (arquivo: 3.2_workflow_atual.md). Preciso de uma análise estratégica para apresentar ao CEO com recomendações concretas de automação com IA.

Execute as 3 etapas abaixo:

**Etapa 1 — Mapeamento do Fluxo**
Leia a descrição do processo e monte um mapa textual do fluxo, no formato:

[ETAPA 1: Nome] → Responsável: X | Tempo médio: Y | Ferramenta atual: Z
    ↓
[DECISÃO: Condição] → Se Sim: próxima etapa | Se Não: caminho alternativo
    ↓
[ETAPA 2: Nome] → ...

Identifique e destaque os pontos de espera (onde o processo fica parado aguardando alguém ou algo) e os pontos de decisão humana (onde um humano precisa avaliar e escolher).

**Etapa 2 — Oportunidades de Substituição por IA**
Para cada etapa do fluxo, avalie se a IA pode:
- **Substituir completamente** (tarefa 100% automatizável)
- **Acelerar significativamente** (IA faz o rascunho, humano valida em <2 min)
- **Não substituir** (requer julgamento humano ou relação pessoal insubstituível)

Para as etapas substituíveis ou aceleráveis, especifique:
- Qual tecnologia de IA usaria (ex: LLM para geração de texto, OCR + IA para leitura de documentos, IA de classificação para triagem)
- Estimativa de redução de tempo (ex: "de 3 horas para 10 minutos")
- Nível de complexidade de implementação: Baixo / Médio / Alto

**Etapa 3 — Arquitetura de Automação Proposta**
Proponha a arquitetura completa de ferramentas para automatizar os principais gargalos identificados. Inclua:

1. **Diagrama de integração** (formato textual):
   [Gatilho] → [Ferramenta de Automação] → [IA] → [Sistema de Destino]

2. **Stack tecnológico recomendado** com justificativa:
   - Ferramenta de automação/orquestração (ex: Zapier, Make, n8n)
   - Modelo(s) de IA (ex: Claude para geração de documentos, GPT para classificação)
   - CRM / ERP de destino (ex: Pipedrive, HubSpot, Salesforce)
   - Integrações específicas necessárias

3. **Roadmap de implementação em 3 fases:**
   - Fase 1 (Semanas 1-4): Quick wins, baixo risco
   - Fase 2 (Meses 2-3): Automações médias com maior impacto
   - Fase 3 (Meses 4-6): Orquestração completa

4. **Projeção de impacto:**
   - Horas/mês economizadas
   - Redução estimada de erros (%)
   - Tempo médio de ciclo atual vs. projetado

Apresente um resumo executivo de 5 linhas no início, com os 3 maiores ganhos que a automação trará para o CEO justificar o investimento.
```
