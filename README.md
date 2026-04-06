# YPO — Avaliação de Ferramentas Agênticas

Repositório de prompts e documentos de apoio para o projeto de benchmarking de ferramentas de IA do grupo YPO.

## Objetivo

Testar e comparar 3 ferramentas agênticas — **Claude Cowork**, **Manus** e **Lindy AI** — em tarefas reais de C-Level, para avaliar qual entrega mais valor em contextos corporativos brasileiros.

O resultado será usado para estruturar um workshop prático para executivos YPO.

---

## Como usar este repositório

Cada task tem uma pasta com:
- O **prompt pronto** para colar na ferramenta
- Os **documentos de apoio** que devem ser anexados junto com o prompt

**Fluxo de teste:**

```
1. Abra TODOS OS PROMPTS.md e copie o prompt da task que você vai testar
2. Acesse a pasta da task e baixe os documentos de apoio
3. Cole o prompt na ferramenta e anexe os documentos indicados
4. Execute e registre o resultado no link abaixo
```

> **Importante:** cole o prompt exatamente como está, sem editar. A ideia é testar as ferramentas sob as mesmas condições.

---

## Estrutura de Arquivos

```
📁 Prompts e Documentos de Apoio/
│
├── TODOS OS PROMPTS.md          ← Todos os 6 prompts em um único lugar
│
├── 📁 Task 1.1/
│   ├── 1.1_email_parceiro.md           ← E-mail + deck de proposta de parceria
│   └── 1.1_tese_de_investimento.md     ← Estratégia e critérios da empresa
│
├── 📁 Task 1.2/
│   └── 1.2_linkedin_export.csv         ← Export de 80 conexões do LinkedIn
│
├── 📁 Task 2.1/
│   └── 2.1_empresas_alvo.md            ← 5 empresas para análise M&A com URLs
│
├── 📁 Task 2.2/
│   ├── 2.2_minuta_contrato_template.docx  ← Contrato com campos em branco
│   ├── 2.2_dados_cliente.md               ← Dados do cliente para preencher
│   └── 2.2_guia_clausulas_risco.md        ← Guia de cláusulas de atenção
│
├── 📁 Task 3.1/
│   ├── 3.1_relatorio_trimestral.md     ← Relatório financeiro Q4 (denso)
│   └── 3.1_noticias_setor.md           ← 8 notícias do setor no período
│
└── 📁 Task 3.2/
    └── 3.2_workflow_atual.md           ← Descrição de processo com 12 etapas
```

---

## As Tasks

### Nível 1 — Eficiência Individual

| Task | O que fazer | Documentos necessários | Dificuldade |
|---|---|---|---|
| **1.1** | Ler e-mail de proposta de parceiro, cruzar com tese da empresa e gerar 3 opções de resposta (recusar / pedir mais dados / aceitar) | `1.1_email_parceiro.md` + `1.1_tese_de_investimento.md` | Baixa |
| **1.2** | Classificar 80 conexões do LinkedIn por setor, identificar "Power Players" (C-suite e Diretores de empresas relevantes) e escrever mensagens de re-aproximação personalizadas | `1.2_linkedin_export.csv` | Baixa/Média |

### Nível 2 — Operações

| Task | O que fazer | Documentos necessários | Dificuldade |
|---|---|---|---|
| **2.1** | Pesquisar 5 empresas na internet, extrair modelo de receita de cada uma e gerar uma tabela SWOT comparativa com ranking de atratividade | `2.1_empresas_alvo.md` | Média |
| **2.2** | Preencher uma minuta de contrato com os dados do cliente, identificar cláusulas de risco e gerar e-mail para o jurídico | `2.2_minuta_contrato_template.docx` + `2.2_dados_cliente.md` + `2.2_guia_clausulas_risco.md` | Média |

### Nível 3 — Orquestração Complexa

| Task | O que fazer | Documentos necessários | Dificuldade |
|---|---|---|---|
| **3.1** | Extrair KPIs de um relatório trimestral, cruzar com sentimento de mercado e montar roteiro de apresentação de 10 slides para o Board | `3.1_relatorio_trimestral.md` + `3.1_noticias_setor.md` | Alta |
| **3.2** | Mapear um processo de 12 etapas, identificar onde IA pode substituir humanos e propor arquitetura de automação (Zapier + IA + CRM) com roadmap e ROI projetado | `3.2_workflow_atual.md` | Alta |

---

## O que avaliar em cada teste

Após executar cada task, registre sua avaliação nos seguintes critérios:

### Critérios de Avaliação

| Critério | Pergunta-guia | Como medir |
|---|---|---|
| **Autonomia** | A ferramenta completou as 3+ etapas sem precisar de intervenção humana? | Sim / Parcial (parou em qual etapa?) / Não |
| **Raciocínio** | O output demonstra que a ferramenta entendeu nuances estratégicas, ou foi superficial? | Ex: na 1.1, ela cruzou os dados do e-mail com a tese, ou gerou respostas genéricas? |
| **Output pronto para uso** | O resultado pode ser usado diretamente (enviado, apresentado, assinado) sem reescrever? | Sim / Precisa de ajustes / Não |
| **Integração** | A ferramenta acessou a internet (task 2.1), leu o .docx (task 2.2) e os outros formatos sem erros? | Descreva o que funcionou e o que falhou |
| **Segurança / Dados** | A ferramenta armazenou, vazou ou mencionou dados sensíveis de forma inadequada? | Sim (descrever) / Não |
| **Tempo de execução** | Quanto tempo levou do início ao output final? | Em minutos |

### Referências de tempo esperado

| Nível | Tempo aceitável |
|---|---|
| Nível 1 | até 5 minutos |
| Nível 2 | até 10 minutos |
| Nível 3 | até 20 minutos |

---

## Registro de Resultados

Registre o output e sua avaliação neste Google Docs (certifique-se que o link está com permissão correta antes de compartilhar):

> 🔗 **[Link da planilha de resultados — preencher aqui]**

Cada testador deve incluir:
- Link para o output gerado (Google Docs, print, PDF — o que a ferramenta gerou)
- Avaliação nos 6 critérios acima
- Campo livre para observações

---

## Distribuição dos Testes

| Ferramenta | Testadores |
|---|---|
| **Claude Cowork** | Carlão, Frazão |
| **Manus** | Marcão, Murilo |
| **Lindy AI** | Roberto, Arruda |

Cada dupla testa **todas as 6 tasks** na sua ferramenta. Prazo: resultados prontos até **quarta-feira, 08/04**.

---

## Dúvidas frequentes

**A ferramenta não aceita .md — o que fazer?**
Copie e cole o conteúdo do arquivo diretamente no chat da ferramenta, antes do prompt. Funciona na maioria das ferramentas agênticas.

**Posso adaptar o prompt se a ferramenta não entender?**
Não — a ideia é testar as ferramentas nas mesmas condições. Se precisar adaptar, anote no campo de observações o que foi necessário mudar e por quê.

**A tarefa é fictícia ou real?**
Os documentos são fictícios mas construídos com dados plausíveis (empresas, CNPJs, valores, estruturas financeiras realistas). O objetivo é simular um cenário real de trabalho de C-Level.

**Onde fica o prompt de cada task?**
Todos os prompts estão no arquivo `TODOS OS PROMPTS.md`. Cada task tem seu próprio bloco de código — basta copiar o conteúdo dentro do bloco.
