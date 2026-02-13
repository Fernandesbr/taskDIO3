📌 Overview

Este projeto consiste na construção de uma planilha avançada em Excel para análise e simulação de receitas recorrentes baseadas em assinaturas (subscription model).

A solução foi desenvolvida com foco em:

Estruturação de base de dados

Aplicação de cálculos financeiros automatizados

Consolidação de indicadores

Visualização executiva em dashboard

Simulação de cenários com base em assinaturas, passes sazonais e cupons

O arquivo principal do projeto está estruturado em múltiplas abas organizadas de forma modular.

🗂 Estrutura da Planilha

O arquivo contém as seguintes abas:

1️⃣ Assets

Objetivo:
Centralizar parâmetros, listas auxiliares e elementos de suporte ao modelo.

Função na arquitetura:

Base para validações de dados

Fonte para listas suspensas

Organização de variáveis reutilizáveis

Controle de categorias e planos

Essa aba funciona como camada de apoio estrutural do modelo.

2️⃣ Bases

Objetivo:
Armazenar a base de dados principal de assinantes.

📌 Estrutura da Base
Campo	Descrição
Subscriber ID	Identificador único do assinante
Name	Nome do assinante
Plan	Tipo de plano contratado
Start Date	Data de início da assinatura
Auto Renewal	Indicador de renovação automática
Subscription Price	Valor da assinatura
Subscription Type	Tipo de cobrança
EA Play Season Pass	Indica se possui passe adicional
EA Play Season Pass Price	Valor do passe EA
Minecraft Season Pass	Indica se possui passe adicional
Minecraft Season Pass Price	Valor do passe Minecraft
Coupon Value	Valor de desconto aplicado
Total Value	Receita final por assinante
🔎 Papel da aba no modelo

Base de entrada de dados

Fonte para cálculos agregados

Alimentação do dashboard

Permite análises como:

Receita total

Receita média por usuário (ARPU)

Receita por tipo de plano

Impacto de cupons

Receita incremental por season pass

3️⃣ Cálculos

Objetivo:
Centralizar fórmulas e indicadores consolidados.

📊 Exemplos de métricas calculadas:

Receita total consolidada

Receita por tipo de assinatura

Receita adicional por season pass

Total de descontos aplicados

Ticket médio

Percentual de renovação automática

📐 Função Arquitetural

Essa aba atua como camada lógica do modelo, separando:

Dados brutos (Bases)

Processamento (Cálculos)

Visualização (Dashboard)

Essa separação melhora:

Organização

Manutenção

Escalabilidade do modelo

Governança da informação

4️⃣ Dashboard

Objetivo:
Apresentar os indicadores de forma visual e executiva.

🎯 Características:

Visão consolidada da receita

Indicadores-chave (KPIs)

Elementos gráficos

Filtros interativos

Segmentação por plano ou tipo de assinatura

👔 Público-alvo:

Gestão

Área financeira

Produto

Estratégia

O dashboard foi projetado para fornecer visão rápida de desempenho e apoiar tomada de decisão.

🏗 Arquitetura da Solução

O modelo segue uma arquitetura em camadas:

Assets (Parâmetros)
        ↓
Bases (Dados Brutos)
        ↓
Cálculos (Processamento)
        ↓
Dashboard (Visualização Executiva)


Essa abordagem reduz riscos de erro e facilita evolução futura.

⚙️ Lógica de Cálculo

O valor total por assinante considera:

Total Value =
Subscription Price
+ EA Play Season Pass Price
+ Minecraft Season Pass Price
- Coupon Value


Os cálculos consolidados utilizam funções como:

SUM

SUMIF / SUMIFS

COUNTIF

AVERAGE

IF

Validação de dados

Referências estruturadas

🚀 Como Utilizar

Inserir ou atualizar dados na aba Bases

Verificar parâmetros em Assets

Validar indicadores na aba Cálculos

Analisar resultados no Dashboard

📈 Possíveis Evoluções

Inclusão de churn rate

Projeção mensal de receita recorrente (MRR)

Simulação de crescimento de base

Integração com Power BI

Automação via Power Query

Controle de cohort

Análise preditiva

🛠 Requisitos

Microsoft Excel 2016+ ou Microsoft 365

Habilitação de cálculos automáticos

Não requer macros

📊 Objetivos do Projeto

Este projeto demonstra:

Modelagem de dados em Excel

Estruturação de solução analítica

Organização em camadas

Criação de dashboard executivo

Aplicação de lógica financeira

Boas práticas de governança de planilhas

📌 Status

✅ Modelo funcional
✅ Estrutura modular
✅ Dashboard implementado
🔄 Possível expansão para análise avançada
