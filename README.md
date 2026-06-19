# Da Planilha ao Pipeline Inteligente

### Camada de IA para Leitura de Documentos, Roteamento e Detecção de Anomalias em uma Indústria de Embalagens






---

# ⚠️ Status do Projeto

**Este sistema está em desenvolvimento e *****não***** está pronto** como parte do Projeto de Aprendizagem Colaborativa (PAC) do Centro Universitário Católica de Santa Catarina.

A proposta consiste em adicionar uma camada de Inteligência Artificial ao ERP da Markaplast, indústria fabricante de embalagens plásticas, com o objetivo de automatizar tarefas operacionais que ainda dependem de intervenção humana.

## Situação Atual

| Módulo                   | Status                |
| ------------------------ | --------------------- |
| ERP Markaplast           | ✅ Em produção         |
| OCR para documentos      | 🚧 Em desenvolvimento |
| Classificação de pedidos | 🚧 Em desenvolvimento |
| Detecção de anomalias    | 🚧 Em desenvolvimento |
| Validação experimental   | 📋 Planejada          |

---

# 🎯 Visão Geral

Antes da implantação do ERP próprio, a Markaplast realizava o controle de pedidos, produção e faturamento por meio de planilhas Excel e documentos Word dispersos entre diferentes setores.

Esse cenário gerava:

* Retrabalho operacional
* Falta de padronização
* Perda de informações
* Divergências entre departamentos
* Dependência excessiva de processos manuais

Embora o ERP tenha centralizado as operações da empresa, três atividades continuam demandando esforço humano significativo:

1. Digitação e redigitação de dados para emissão fiscal;
2. Priorização manual de pedidos de produção;
3. Conferência de divergências fiscais e financeiras.

O objetivo deste projeto é reduzir esses gargalos através da aplicação de Inteligência Artificial integrada diretamente ao sistema já utilizado pela empresa.

---

# 🧠 Como Funciona a Camada de IA

A solução proposta é composta por três módulos principais.

## 1. OCR para Leitura de Documentos

Responsável pela leitura automática de:

* Pedidos de venda
* Notas fiscais
* PDFs
* Imagens digitalizadas

### Objetivos

* Eliminar digitação manual
* Reduzir erros de transcrição
* Automatizar o preenchimento de cadastros
* Gerar informações para emissão de NF-e

---

## 2. Classificação e Roteamento de Pedidos

Utiliza algoritmos de Machine Learning para analisar os dados do pedido e determinar:

* Prioridade de produção
* Encaminhamento correto do fluxo
* Estado operacional adequado

### Benefícios

* Padronização das decisões
* Menor dependência de operadores experientes
* Maior velocidade de processamento

---

## 3. Detecção de Anomalias

Analisa históricos de pedidos e notas fiscais para identificar:

* Valores inconsistentes
* Tributação incorreta
* Divergências financeiras
* Pedidos fora do comportamento esperado

### Objetivo

Antecipar problemas que atualmente só são identificados durante conferências manuais.

---

# 🏗️ Arquitetura da Solução

```text
Usuários
    │
React + Vite
    │
FastAPI
    │
PostgreSQL
    │
─────────────────────────
      Camada de IA
─────────────────────────

OCR de Documentos
        ↓
Classificação de Pedidos
        ↓
Detecção de Anomalias
```

A camada de Inteligência Artificial atua de forma complementar ao ERP já existente, sem necessidade de reescrever a plataforma principal.

---

# 🛠️ Tecnologias Utilizadas

| Camada         | Tecnologia                   |
| -------------- | ---------------------------- |
| Backend        | Python + FastAPI             |
| Frontend       | React + Vite                 |
| Banco de Dados | PostgreSQL                   |
| OCR            | Processamento de Imagens     |
| IA             | Machine Learning             |
| Integrações    | Focus NFe, ViaCEP, BrasilAPI |

---

# 📊 Resultados Esperados

A validação experimental do projeto pretende medir:

| Indicador                | Objetivo                    |
| ------------------------ | --------------------------- |
| Precisão da extração OCR | Alta taxa de acerto         |
| Classificação de pedidos | Accuracy e F1 elevados      |
| Detecção de anomalias    | Precision e Recall elevados |
| Tempo operacional        | Redução significativa       |

Os resultados serão obtidos através de experimentos realizados com dados reais da empresa.

---

# 🚀 Inovação

O diferencial da proposta não está na utilização isolada de OCR, classificação ou detecção de anomalias.

A inovação consiste em integrar essas três tecnologias dentro de um único fluxo operacional conectado a um ERP industrial em funcionamento, permitindo:

* Decisões rastreáveis;
* Redução de atividades manuais;
* Maior eficiência operacional;
* Conformidade fiscal durante a emissão de NF-e.

---

# 🗺️ Roadmap

## Fase 1 — OCR

* Coleta de documentos
* Rotulação de dados
* Integração ao ERP

## Fase 2 — Classificação

* Desenvolvimento do classificador
* Priorização automática
* Roteamento inteligente

## Fase 3 — Detecção de Anomalias

* Modelagem dos dados históricos
* Treinamento dos algoritmos
* Identificação de inconsistências

## Fase 4 — Validação

* Execução dos experimentos
* Coleta de métricas
* Análise dos resultados

---

# ⚠️ Limitações

* Projeto ainda não validado experimentalmente.
* Dependência da qualidade dos documentos digitalizados.
* Necessidade de revisão humana em processos fiscais críticos.
* Dependência de dados históricos para treinamento dos modelos.
* Possibilidade de ajustes futuros conforme os resultados obtidos durante o PAC.

---

# 🎓 Contexto Acadêmico

Este repositório representa a proposta de portfólio desenvolvida para a disciplina Projeto de Aprendizagem Colaborativa (PAC), do Centro Universitário Católica de Santa Catarina.

O trabalho propõe a aplicação prática de Inteligência Artificial em processos industriais reais, utilizando como estudo de caso a empresa Markaplast.
