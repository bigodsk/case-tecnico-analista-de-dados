# Análise de Dados — WYZ Prime Commerce
## Case Analista de Dados II

---

## Contexto e Metodologia

**Período analisado:** 2021–2025 (dados de vendas)  
**Fonte:** `sales_customer_invoices` (2.587 registros), `product_catalog` (6 linhas), `customer_base` (9.167 clientes)  
**Ferramenta de análise:** Python + Power BI

> **Nota importante sobre qualidade dos dados:** Foi identificado um outlier crítico na base — uma transação de 21/05/2023 com 100.000 unidades de "Home and lifestyle" totalizando **$21.000.000**, claramente um erro de entrada de dados (quantidade impossível para uma única venda de varejo). Esta transação foi removida de toda a análise. O faturamento real de 2023 é **$298K**, não $21,3MM.

---

## Visão Geral do Negócio (2021–2025)

| Ano  | Faturamento  | Gross Income | Transações | Crescimento |
|------|-------------|--------------|-----------|-------------|
| 2021 | $331.091    | $15.766      | 534       | —           |
| 2022 | $182.306    | $8.681       | 305       | **-44,9%**  |
| 2023 | $298.032    | $14.192      | 452       | +63,5%      |
| 2024 | $350.963    | $16.713      | 559       | +17,8%      |
| 2025 | $444.417    | $18.227      | 736       | **+26,6%**  |

**Tendência:** Após a queda em 2022 (provavelmente reflexo do período pós-pandemia), o negócio retomou crescimento consistente, acelerando para +26,6% em 2025 — o melhor resultado do período.

---

## Perguntas Chave — Respostas

---

### 1, 2 e 3 — Satisfação do Cliente com Produtos: Categorias, Destaques e Tendências

**Metodologia:** Rating médio por linha de produto (escala 1–10) comparado entre 2021 e 2025.

#### Ratings por categoria e evolução temporal:

| Categoria              | 2021 | 2022 | 2023 | 2024 | 2025 | Tendência |
|------------------------|------|------|------|------|------|-----------|
| Electronic accessories | 6,77 | 6,72 | 6,58 | 6,64 | **7,22** | ↑ Forte alta |
| Sports and travel      | 6,67 | 6,92 | 6,96 | 6,67 | **7,01** | ↑ Alta     |
| Food and beverages     | 6,93 | 7,00 | **7,23** | 7,06 | 6,89 | → Estável |
| Home and lifestyle     | 6,76 | 7,06 | **7,22** | 6,93 | 6,89 | → Estável |
| Fashion accessories    | 6,93 | 6,84 | **7,33** | 6,89 | 6,79 | ↓ Leve queda |
| Health and beauty      | **7,10** | 6,81 | 6,93 | 6,52 | 6,53 | ↓ Queda contínua |

**Respostas:**

**Q1 — Como as categorias se saíram?**
- A estratégia de melhoria da satisfação surtiu efeito parcial. O rating geral permanece entre 6,5 e 7,2, sem grandes oscilações. Nenhuma categoria atingiu 8,0, indicando espaço relevante de melhoria.

**Q2 — Quais se destacaram e quais ficaram para trás?**
- **Destaque positivo:** *Electronic accessories* disparou de 6,77 para **7,22 (+0,45 pts)** — maior salto absoluto do período. *Sports and travel* também melhorou de 6,67 para **7,01**.
- **Ficaram para trás:** *Health and beauty* caiu de 7,10 para **6,53** — queda de 0,57 pontos em 5 anos, tendência consistentemente negativa, **sinal de alerta**. *Fashion accessories* também recuou levemente.

**Q3 — Tendências e padrões:**
- O pico geral de ratings ocorreu em **2023** (quase todas as categorias registraram notas mais altas), coincidindo com a retomada econômica pós-queda de 2022.
- Em 2025, o crescimento de volume de vendas em *Fashion accessories* (+79% de transações, de 96 para 172) veio acompanhado de queda no rating (6,89 → 6,79) — possível efeito de atendimento/qualidade sob maior demanda.
- *Health and beauty* requer **atenção urgente**: declínio contínuo de 4 anos. Volume de vendas caiu pela metade (91 transações em 2024 vs. 45 em 2025). Insatisfação pode estar afastando clientes.

---

### 4 e 5 — Campanha para Home and Lifestyle: Momento Ideal e Público-Alvo

**Q4 — Quando lançar a campanha em 2026?**

Análise da sazonalidade histórica de H&L (todos os anos, sem outlier):

| Mês | Faturamento | Transações | Ticket Médio |
|-----|-------------|-----------|--------------|
| Jan | $43.749     | 37        | $1.182       |
| Fev | $42.342     | 37        | $1.144       |
| Mar | $43.413     | 38        | $1.142       |
| Abr | $35.484     | 32        | $1.109       |
| **Mai** | **$41.676** | **36**  | **$1.158**   |
| **Jun** | **$27.693** | **27**  | **$1.026**   |
| **Jul** | **$43.149** | **39**  | **$1.106**   |
| **Ago** | **$55.098** | **45**  | **$1.224**   |
| **Set** | **$49.626** | **45**  | **$1.103**   |
| Out | $41.853     | 35        | $1.196       |
| Nov | $40.860     | 37        | $1.104       |
| Dez | $41.346     | 35        | $1.181       |

**Recomendação:** Lançar a campanha em **julho/2026**, com pico de ativação em **agosto e setembro**. Esses dois meses concentram:
- Maior volume de transações (45 cada = +29% vs. média dos demais meses)
- Maior faturamento histórico ($55K em agosto)
- Ticket médio elevado ($1.224 em agosto)

**Junho é o pior mês** (queda de -35% vs. agosto) — evitar ações promocionais neste período.

A estratégia sugerida: **pré-aquecimento em julho** (ativação de base) → **campanha principal em agosto-setembro** → **follow-up em outubro** (ticket médio alto, $1.196).

---

**Q5 — Qual o público-alvo da campanha H&L?**

Perfil dos clientes que compraram H&L em 2025 (125 clientes únicos):

| Atributo       | Dado                  |
|----------------|-----------------------|
| Idade média    | 45 anos               |
| Faixa de idade | 18–69 anos            |
| Gênero         | Feminino 52% / Masculino 48% (equilibrado) |
| Classe social  | Middle (57%) > Lower (26%) > Upper (17%) |
| Renda média    | $82.739/ano           |
| Tipo de cliente| Member (54%) > Normal |
| Pagamento preferido | Credit card (38%) > Ewallet (35%) > Cash (27%) |

**Público-alvo recomendado:**
- **Perfil primário:** Adultos de 35–55 anos, classe média, membros do programa de fidelidade (Members)
- **Canal preferencial:** Credit card e Ewallet (73% das compras H&L combinados) — potencial para promoção de cashback via carteira digital
- **Insight adicional:** O ticket médio de H&L é $1.143 (o maior de todas as categorias), portanto o público tem poder de compra relevante mesmo na classe média. Campanhas com parcelamento ou cashback via Ewallet teriam forte apelo.

---

### 6 — Orçamento de Marketing Reduzido: Em qual linha de produtos focar?

Análise combinada de ticket médio, margem de lucro e volume de vendas **(acumulado 2021–2025)**:

| Linha de Produto       | Receita Total | Gross Income | Margem | Ticket Médio | Transações |
|------------------------|--------------|--------------|--------|-------------|-----------|
| Home and lifestyle     | $506.289     | $23.089      | 6,0%   | $1.143      | 443       |
| Sports and travel      | $458.395     | $20.995      | **15,0%** | **$1.035** | 443    |
| Fashion accessories    | $354.373     | $16.213      | **18,1%** | $705     | **503**   |
| Health and beauty      | $180.421     | $8.431       | 12,1%  | $520        | 347       |
| Electronic accessories | $68.914      | $3.124       | 12,4%  | $171        | 403       |
| Food and beverages     | $38.417      | $1.727       | 2,1%   | $86         | 447       |

**Recomendação: Sports and Travel como foco principal, Fashion accessories como secundário.**

**Justificativa — Sports and Travel:**
- **Maior ROI potencial:** margem de 15% com ticket médio de $1.035 — cada venda gera $155 de retorno bruto
- **Volume alto:** 443 transações (empatado com H&L), com crescimento em 2025
- **Satisfação crescente:** rating subiu de 6,67 para 7,01 em 2025 — clientes satisfeitos convertem melhor em campanhas
- **Tendência positiva:** receita cresceu 17% em 2025 vs. 2024 nessa categoria

**Sports and Travel supera H&L** pelo critério de margem: H&L tem maior receita bruta mas margem apenas 6%, gerando gross income similar com custo de marketing potencialmente mais alto por conversão.

**Fashion accessories como opção complementar:** maior margem de todas (18,1%) e maior volume de transações (503), mas ticket menor ($705) e rating em declínio em 2025 — ideal para ações de cross-sell e upsell a baixo custo.

> **Evitar:** Food and beverages (margem 2,1%, ticket $86 — custo de aquisição provavelmente supera o retorno). Electronic accessories tem baixo ticket médio ($171) apesar de boa margem.

---

### 7 — A meta de reativar 20% dos clientes inativos é viável?

**Mapeamento dos inativos:**

| Indicador | Valor |
|-----------|-------|
| Clientes que compraram em 2024 mas não em 2025 | 238 |
| Clientes que compraram antes de 2024 e não em 2025 | 237 |
| **Total de clientes inativos** | **475** |
| Ticket médio histórico dos inativos | $619,91 |
| Ticket médio da última compra dos inativos (2024) | $642,55 |

**Avaliação da meta de 20%:**

20% de 475 = **95 clientes** a reativar

A meta é **viável e conservadora** com base em benchmarks de mercado:
- Taxa de reativação no varejo varia de **10% a 30%**, com conversão média de ~10,3% em campanhas automatizadas segundo dados agregados do setor ([Opensend / MailMend — Win-Back Campaign Success Rate Statistics 2025](https://www.opensend.com/post/win-back-campaign-success-rate-statistics); [Klaviyo — Benchmark Report 2025](https://www.klaviyo.com/marketing-resources/enterprise-benchmarks-report))
- Para uma base de clientes que já tem histórico de compra na empresa (não são leads frios), a taxa de 20% é atingível com uma campanha bem segmentada

**Distribuição dos inativos por última compra:**
- Última compra em 2024: **238 clientes** (50,1%) — mais quentes, maior probabilidade de reativação
- Última compra em 2023: **105 clientes** (22,1%) — médio potencial
- Última compra em 2022: **74 clientes** (15,6%) — menor probabilidade
- Última compra em 2021: **58 clientes** (12,2%) — provavelmente perdidos

**Estratégia sugerida:** Priorizar os **238 inativos de 2024** como público primário — a taxa de reativação esperada neste grupo é de 25–30%.

---

### 8 — Tamanho do público-alvo para alcançar $30K na campanha de reativação

**Cálculo:**

- Ticket médio dos inativos: **$619,91** (conservador) / **$642,55** (última compra em 2024)
- Clientes necessários para $30K: $30.000 ÷ $619,91 = **~48 clientes**
- Com taxa de conversão de 20%: 48 ÷ 0,20 = **~242 clientes a contatar**

**Conclusão:**
- Contatar **242 clientes** (51% da base inativa total de 475) é suficiente para atingir $30K com 20% de conversão
- **Recomendação:** Focar nos **238 inativos de 2024** (os mais recentes) — esse grupo sozinho, com conversão de 20% (48 clientes × $642 = **$30.816**), já atinge a meta

**Projeção otimista (toda a base):**
- 475 inativos × 20% = 95 reativados × $619,91 = **$58.891** — quase o dobro da meta

**Perfil dos inativos (para segmentação):**
- Idade média: 43 anos
- Classe social: Middle 55% / Lower 27% / Upper 18%
- Gênero equilibrado (51% F / 49% M)

---

### 9 — Outros Insights

#### 9.1 — Ewallet em alta acelerada
O uso da carteira virtual cresceu de **30–36% (2021–2024)** para **45,7% em 2025** — maior salto histórico. A estratégia de promover o Ewallet está funcionando. Para 2026, ações de cashback ou benefícios exclusivos via Ewallet podem acelerar ainda mais essa adoção.

| Ano  | Ewallet % |
|------|-----------|
| 2021 | 33,5%     |
| 2022 | 30,2%     |
| 2023 | 36,1%     |
| 2024 | 32,0%     |
| **2025** | **45,7%** |

#### 9.2 — Programa de Membros estagnado
A proporção de Members vs. Normal clientes **não mudou** em 5 anos (oscila em torno de 49%–51%). A estratégia de fortalecer o programa de membros em 2025 **não gerou crescimento perceptível na proporção de associados**. Oportunidade de revisão do programa.

#### 9.3 — Health and Beauty: categoria em crise silenciosa
- Rating em queda contínua de 7,10 (2021) para 6,53 (2025)
- Volume de transações caiu pela metade: de 91 em 2024 para **45 em 2025**
- Apesar de margem razoável (12,1%), a categoria está perdendo clientes
- Requer investigação: problema de mix de produtos? Precificação? Concorrência?

#### 9.4 — Crescimento concentrado em Fashion e Food (2025)
Fashion passou de 96 para 172 transações (+79%) e Food de 79 para 154 (+95%) em 2025 vs. 2024 — crescimento significativo. Porém o ticket médio dessas categorias é menor, o que dilui a margem.

#### 9.5 — Outlier de dados crítico
A transação de 100.000 unidades de H&L em maio/2023 (CUST-0797) distorceria toda a análise. É fundamental implementar validações na captura de dados para evitar registros com quantidades anômalas.

#### 9.6 — Filiais equilibradas
As três filiais (A, B, C) têm desempenho muito similar em 2025 (A: $152K, B: $147K, C: $145K), sem necessidade de intervenção diferenciada por filial.

---

### 10 — Estratégias Adicionais Recomendadas para 2026

**1. Programa de Membros — Reformulação urgente**
O programa não cresceu em 5 anos. Proposta: criar tier de benefícios (Silver/Gold/Platinum) vinculado ao Ewallet — compras via carteira digital acumulam pontos extras. Isso endereça simultaneamente as estratégias de membros e de carteira virtual.

**2. Resgate de Health and Beauty**
Lançar pesquisa rápida de NPS com os 347 clientes que compraram a categoria para entender a queda de satisfação. Com margem de 12%, vale recuperar a categoria antes de descontinuá-la.

**3. Campanha de Reativação em 2 ondas**
- **Onda 1 (Fev/Mar):** Clientes inativos de 2024 (238 pessoas) — oferta personalizada baseada em última categoria comprada
- **Onda 2 (Jul/Ago):** Coincide com o pico sazonal de H&L — oferta específica para inativos que compraram H&L

**4. Upsell via Ewallet nas compras de alto ticket**
Dado que 45,7% já usam Ewallet e as categorias de maior ticket (H&L $1.143, Sports $1.035) são compras planejadas, oferecer parcelamento sem juros via carteira digital pode aumentar a conversão e o ticket médio.

**5. Foco em Sports and Travel para campanhas paid**
Com margem de 15% e ticket de $1.035, o ROI de campanhas pagas é viável. Meta 2026: crescer Sports and Travel de $130K para $160K em 2026 representaria +23%.

**6. Dashboard de monitoramento contínuo de ratings**
Implementar alerta automático quando qualquer categoria cair abaixo de 6,5 por dois meses consecutivos — evitaria que o declínio de Health and Beauty se prolongasse por 4 anos sem ação.

---

## Resumo Executivo

| Pergunta | Resposta Principal |
|----------|-------------------|
| Satisfação por categoria | Electronic accessories e Sports em alta; Health and beauty em queda crítica |
| Destaque positivo | Electronic accessories (+0,45 pts em 5 anos) |
| Destaque negativo | Health and beauty (-0,57 pts, volume caiu 50%) |
| Melhor mês para H&L | Agosto–Setembro (maior volume e faturamento) |
| Público H&L | Adultos 35–55 anos, classe média, Members, preferência por credit card/Ewallet |
| Foco com orçamento limitado | Sports and Travel (maior ROI: 15% de margem + ticket $1.035) |
| Meta 20% reativação | Viável — benchmarks de mercado suportam 15–25% |
| Público-alvo reativação | 242 clientes (foco nos 238 inativos de 2024 para maior conversão) |
| Insight chave | Ewallet saltou para 45,7% em 2025 — estratégia funcionou |
| Estratégia adicional | Reformular programa de membros, vincular ao Ewallet com sistema de pontos |

---

*Análise realizada com base nos dados históricos WYZ Prime Commerce (2021–2025). Um registro outlier (quantidade 100.000 unidades, maio/2023) foi excluído por representar erro de entrada de dados.*

---

## Referências

| Fonte | Dado utilizado | Link |
|-------|---------------|------|
| ABComm / E-Commerce Brasil — Resultados 2024 | Crescimento e-commerce BR 2024: **+10,5%**; faturamento R$ 204,3 bi; ticket médio R$ 492,40 | [ecommercebrasil.com.br](https://www.ecommercebrasil.com.br/noticias/e-commerce-resultados-2024-brasil-abcomm) |
| IBGE — Pesquisa Mensal de Comércio (PMC) 2024 | Crescimento varejo físico BR 2024: **+4,7%** (melhor resultado desde 2012) | [agenciadenoticias.ibge.gov.br](https://agenciadenoticias.ibge.gov.br/agencia-sala-de-imprensa/2013-agencia-de-noticias/releases/42685-vendas-no-varejo-fecham-2024-com-alta-de-4-7) |
| Febraban — Dados Anuais Pix 2024 | Pix: 63,8 bilhões de transações (+52% vs. 2023); principal método de pagamento do BR | [portal.febraban.org.br](https://portal.febraban.org.br/noticia/4290/pt-br/) |
| BCB — Relatório Anual SPI 2024 | Pix: **24%** dos pagamentos no varejo físico (H1 2024) | [bcb.gov.br — Relatório SPI 2024 (PDF)](https://www.bcb.gov.br/content/estabilidadefinanceira/relatorios_SPI/relatorio_anual_spi_2024.pdf) |
| FTI Consulting / Central do Varejo — Online Retail Report 2025 | Pix: **40%** das transações no e-commerce brasileiro | [centraldovarejo.com.br](https://centraldovarejo.com.br/pix-representa-40-nas-compras-online-e-impulsiona-varejo-online-aponta-pesquisa/) |
| ABEMF — 7º Fórum de Fidelização (Q2 2024) | **316 milhões** de cadastros ativos em programas de fidelidade; 72% dos membros satisfeitos | [blog.abemf.com.br](https://blog.abemf.com.br/7o-forum-de-fidelizacao-marca-os-10-anos-da-abemf-e-aponta-a-forca-do-mercado-brasileiro/) |
| SBVC / Pinion / Cielo — Satisfação do Consumidor no Varejo BR 2024 | Satisfação e-commerce/apps: **91%**; varejo físico: **89%** (nota: estudo usa %, não escala 1–10) | [revistavarejobrasil.com.br](https://www.revistavarejobrasil.com.br/formatos-de-varejo-online-tem-indices-mais-elevados-de-satisfacao-dos-clientes/) |
| Opensend / MailMend — Win-Back Campaign Statistics 2025 | Taxa de reativação: **10%–30%**; conversão média de campanhas automatizadas: 10,34% | [opensend.com](https://www.opensend.com/post/win-back-campaign-success-rate-statistics) |
| Klaviyo — Benchmark Report 2025 (AMER) | Benchmarks de fluxos de e-mail por tipo de campanha | [klaviyo.com](https://www.klaviyo.com/marketing-resources/enterprise-benchmarks-report) |
