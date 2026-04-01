# WYZ Prime Commerce — Case Técnico de Análise de Dados

Análise exploratória completa de dados de varejo para a empresa fictícia **WYZ Prime Commerce**, com foco em satisfação de clientes, estratégia de campanha, alocação de orçamento de marketing e reativação de clientes inativos.

---

## Estrutura do Repositório

```
├── analise_wyz_prime.ipynb     # Notebook principal com toda a análise
├── data/
│   ├── WYZ Prime Commerce.xlsx # Base de dados original (4 abas)
│   ├── pbi_sales_clean.csv     # Vendas limpas para Power BI
│   ├── pbi_clientes_inativos.csv
│   ├── pbi_produto_ano.csv
│   ├── pbi_hl_calendario.csv
│   └── pbi_rfm_clientes.csv
├── figures/                    # Gráficos gerados pelo notebook (23 figuras)
└── docs/
    └── analise_case_wyz_prime.md   # Análise narrativa com respostas às 10 questões
    
```

---

## Dados

A base contém dados de **2021 a 2025** de uma rede de varejo com 3 filiais (A, B, C), cobrindo:

- **2.587 transações** de vendas (2.586 após remoção de outlier)
- **9.167 clientes** cadastrados
- **6 linhas de produto**: Electronic accessories, Fashion accessories, Food and beverages, Health and beauty, Home and lifestyle, Sports and travel

---

## Metodologia

### Tratamento de Dados
- Detecção de outliers via **IQR** e **Z-score** (convergência em 1 registro: qty=100.000, total=$21M)
- Remoção validada por critério de negócio (qty máxima legítima = 10)

### Análises Realizadas
- **EDA Geral**: evolução de faturamento, mix de pagamentos, perfil de clientes
- **Satisfação (Q1–Q3)**: rating por categoria, evolução temporal, alertas
- **Campanha Home & Lifestyle (Q4–Q5)**: sazonalidade mensal, perfil de público-alvo
- **Score de Marketing (Q6)**: score composto com pesos — Margem 40% + Ticket 35% + Volume 25%
- **Reativação de Inativos (Q7–Q8)**: segmentação por recência (2024/2023/2022/2021), viabilidade da meta de $30K
- **Análise RFM**: 10 segmentos de clientes com plano de ação por segmento
- **Benchmarking**: comparação com dados públicos (BCB 2024, Klaviyo 2024, ABEMF 2024, ABComm/IBGE 2024)

---

## Como Executar o Notebook

```bash
# Instalar dependências
pip install pandas numpy matplotlib seaborn scipy openpyxl

# Executar o notebook
jupyter notebook analise_wyz_prime.ipynb
```

> O notebook já vem executado com todas as saídas e figuras embutidas. Para re-executar do zero, coloque o arquivo `WYZ Prime Commerce.xlsx` no mesmo diretório do notebook (ou ajuste o caminho na célula de carregamento de dados).

---

## Dashboard Power BI

Os arquivos CSV em `data/` são as fontes prontas para importação no Power BI Desktop. Consulte `docs/guia_powerbi.md` para instruções completas, incluindo:

- Modelo de dados (5 tabelas, relacionamentos)
- 21 medidas DAX com código completo
- Estrutura das 5 páginas do dashboard
- Tema JSON customizado

O arquivo `docs/dashboard_mockup.html` é um protótipo interativo — basta abrir no navegador para visualizar o layout proposto.

---

## Principais Resultados

| Indicador | Valor |
|-----------|-------|
| Faturamento 2025 | $350.399 |
| Crescimento YoY (2024→2025) | +26,6% |
| Ticket Médio | $322 |
| Rating Médio | 6,92/10 |
| Clientes Inativos (sem compra em 2025) | 475 (39% da base) |
| Receita projetada — reativação 20% | $30.590 ✅ Meta atingida |
| Melhor mês para campanha H&L | Agosto/Setembro |
| Categoria com maior score de marketing | Food and beverages |

---

## Tecnologias

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)
![pandas](https://img.shields.io/badge/pandas-2.x-blue)
![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow?logo=powerbi)
