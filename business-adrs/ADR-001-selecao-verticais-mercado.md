---
adr_id: "ADR-001"
title: "Seleção e Priorização das 3 Verticais Estratégicas de Mercado B2B"
status: "APROVADO POR UNANIMIDADE"
date: "2026-10-25"
author: "Adriana (Estratégia de Negócios, Produto & Farmácia)"
deciders:
  - "Adriana (Estratégia & Farmácia)"
  - "Anderson (Dados & Cloud)"
  - "Antônio (Engenharia de IA)"
  - "André (Jurídico & Governança)"
---

# 📈 ADR-001: Seleção das 3 Verticais de Mercado e Modelo de Receita B2B

## 1. Contexto e Problema de Negócio
A **Fratuci Labs** reúne quatro competências complementares raras em uma única família: **Engenharia de Dados de Alta Performance (Anderson)**, **Engenharia de Agentes de IA (Antônio)**, **Direito Digital & Governança (André)** e **Estratégia Empresarial & Ciências Farmacêuticas (Adriana)**.

Precisamos definir em quais mercados B2B concentraremos nossa energia e nossa cota de infraestrutura enxuta (US$ 100/mês no GCP) para atingir **Receita Recorrente Mensal (MRR)** com alta margem bruta e barreiras regulatórias que impeçam concorrentes amadores.

---

## 2. Análise Comparativa das 3 Verticais Selecionadas

| Critério Estratégico | 🏥 Vertical 1: HealthTech & Pharma AI | ⚡ Vertical 2: Data/Stream Ops & AI Readiness | 🚚 Vertical 3: LogTech & Risk Intelligence |
| :--- | :--- | :--- | :--- |
| **Produto Principal** | Copiloto de Triagem de Interações Medicamentosas (DCB/DCI), Auditoria de Prescrições e POPs Digitais Anvisa. | Plataforma Analítica em Tempo Real (ClickHouse ARM64) + Camada RAG Auditável com FinOps Garantido. | Monitoramento Preditivo de Cadeia Fria (*Cold Chain* Farmacêutica), Estoque Crítico e Risco Operacional. |
| **Cliente Ideal (ICP)** | Redes de farmácias, farmácias de manipulação, clínicas multiprofissionais e healthtechs. | Empresas médias de tecnologia, fintechs e varejistas com alto custo de nuvem. | Distribuidoras de medicamentos, operadores logísticos hospitalares e transportadoras. |
| **Diferencial Injusto da Família** | Domínio Farmacêutico (**Adriana**) + Travas LGPD/Responsabilidade Civil (**André**) + Agentes RAG (**Antônio**). | Especialização profunda em ClickHouse 26.x ARM64 e GCP FinOps (**Anderson**). | Combinação de telemetria em tempo real (**Anderson**) + regras sanitárias de transporte (**Adriana**). |
| **Modelo de Receita** | **SaaS B2B Assinatura Mensal** por unidade/farmácia + taxa por volume de auditorias API. | **Retainer Mensal de Plataforma (DataOps-as-a-Service)** + licenciamento de aceleradores. | **SaaS B2B por frota/centro de distribuição** + módulo de compliance contratual. |
| **Ticket Médio Estimado (B2B)** | R$ 1.500 a R$ 8.000 / mês por rede/clínica | R$ 10.000 a R$ 25.000 / mês por operação | R$ 5.000 a R$ 15.000 / mês por distribuidora |
| **Custo Marginal de Nuvem** | **Ultra-Baixo** (< US$ 5/mês por cliente usando Gemini Flash + Cache JSON). | **Baixo** (Infra dedicada paga pelo cliente ou multi-tenant otimizado). | **Baixo** (Ingestão otimizada em Go + compressão ZSTD no ClickHouse). |

---

## 3. Matriz de Pontuação Ponderada (1 a 5)

| Dimensão (Peso) | 🏥 HealthTech & Pharma AI | ⚡ Data/Stream Ops | 🚚 LogTech & Cadeia Fria |
| :--- | :---: | :---: | :---: |
| **Sinergia entre os 4 Sócios (30%)** | **5.0** | 4.0 | 4.5 |
| **Barreira de Entrada Regulatória / Moats (25%)** | **5.0** *(Anvisa + LGPD)* | 3.5 | 4.5 |
| **Velocidade de MVP com Cota de US$ 100 (25%)** | **5.0** | **5.0** | 4.0 |
| **Potencial de Receita Recorrente B2B (20%)** | 4.5 | **5.0** | 4.5 |
| **NOTA FINAL PONDERADA** | **🥇 4.90 / 5.00** | **🥈 4.38 / 5.00** | **🥉 4.38 / 5.00** |

---

## 4. Decisão Estratégica da Diretoria
1. **Carro-Chefe de Produto (MVP Imediato):** Lançar o **Motor de Triagem Farmacológica & Compliance Sanitário (Vertical 1)**, aproveitando a curadoria direta da **Adriana** na base `interacoes-medicamentosas-criticas.json` e o System Prompt blindado pelo **André** e pelo **Antônio**.
2. **Motor de Caixa Rápido (Consultoria Productized):** Ofertar a arquitetura **Data/Stream Ops em ClickHouse ARM & FinOps (Vertical 2)** liderada pelo **Anderson** para financiar a expansão comercial sem necessidade de capital externo.
3. **Expansão Cruzada (Q1/Q2):** Conectar o motor de eventos do **Anderson** com as regras sanitárias da **Adriana** para atacar a **Logística Farmacêutica e Cadeia Fria (Vertical 3)**.
