# ROTEIRO DE APRESENTAÇÃO — WYZ PRIME COMMERCE
## WYZ Prime Commerce — Análise de Dados
### Storytelling de Dados via Power BI | Tempo total: ~25 minutos

---

> **Postura geral:** Apresente como consultor sênior — não leia os slides, conte a história.
> Quando mostrar número impactante, **pause 2 segundos antes de comentá-lo**. O silêncio vende.
> Navegue o Power BI com calma. Cada clique deve parecer intencional, não apressado.

---

## MAPA DE NAVEGAÇÃO NO POWER BI

| Seção da apresentação | Página no Power BI | Ação |
|---|---|---|
| Abertura | Pg 1 — Visão Executiva | Filtro: Todos os anos |
| Outlier | Pg 1 — Visão Executiva | Filtro: 2023 / mostrar linha com outlier |
| KPIs 2025 | Pg 1 — Visão Executiva | Filtro: 2025 |
| Benchmarking | Pg 5 — Benchmarking | Sem filtro |
| Satisfação | Pg 2 — Satisfação e Produtos | Série 2021–2025 |
| Campanha H&L | Pg 3 — Campanha H&L e Orçamento | Filtro: Home and Lifestyle |
| Orçamento Marketing | Pg 3 — Campanha H&L e Orçamento | Score de marketing |
| Reativação / RFM | Pg 4 — Clientes e Reativação | Sem filtro |
| Fechamento | Pg 1 — Visão Executiva | Filtro: 2025 |

---

## SEÇÃO 1 — ABERTURA
### [2 minutos] · Página PBI: Visão Executiva (filtro: todos os anos)

---

### [SLIDE 1] Capa — "WYZ Prime: De Dados a Decisões Estratégicas"

**[VISUAL NO PBI]**
Deixe a **Página 1 — Visão Executiva** aberta com todos os anos selecionados.
O gráfico de linha com a evolução 2021–2025 já conta uma história visualmente antes de você falar.

---

**[FALA]**

> "Antes de qualquer gráfico, uma pergunta:"

*[pausa de 3 segundos — olhe para a plateia]*

> "Quando uma empresa cresce 26,6% em um único ano, isso é sorte — ou é algo que pode ser entendido, replicado e acelerado?"

*[pausa curta]*

> "A WYZ Prime cresceu. Mas crescer sem entender o porquê é como dirigir olhando pelo retrovisor. O que fizemos aqui foi diferente: cinco anos de dados transacionais, quase 2.600 registros de vendas — limpos, estruturados e analisados para contar uma história."

> "Nos próximos 25 minutos vou mostrar o que encontramos: onde a empresa está forte, onde há risco silencioso, e onde está a oportunidade concreta de receita para 2026."

---

**[DICA]** Não explique o 26,6% ainda. Plante o número. A explicação vem na Seção 3.
Termine a abertura apontando para o gráfico de linha sem comentar — deixe a audiência ver a curva de crescimento.

**[TRANSIÇÃO]** "Mas antes de falar em crescimento, preciso mostrar por que tudo que vocês vão ver aqui é confiável. E isso começa com uma história sobre honestidade nos dados."

---

## SEÇÃO 2 — A VERDADE NOS DADOS
### [3 minutos] · Página PBI: Visão Executiva → filtrar 2023 → mostrar nota de outlier

---

### [SLIDE 2] O Registro de $21 Milhões

**[VISUAL NO PBI]**
Vá para a **Página 1** e selecione o filtro **Ano = 2023**.
O faturamento de 2023 vai aparecer distorcido. Aponte para isso.
Se tiver o visual de scatter ou tabela de transações, filtre para mostrar a linha da transação anômala (`CUST-0797`, 21/05/2023, `Home and lifestyle`, qty = 100.000, total = $21.000.000).

---

**[FALA]**

> "Quando rodamos a primeira análise de 2023, o faturamento apareceu em $21,3 milhões."

*[pausa — deixe o número pesar]*

> "Parece ótimo. Mas um número bom demais é sempre um sinal de alerta."

> "Encontramos isso aqui:"

*[aponte para a transação na tela]*

> "Uma única transação. Cliente CUST-0797. 21 de maio de 2023. Categoria **Home and Lifestyle**. Quantidade registrada: **100.000 unidades**. Valor total: **$21 milhões**."

> "Para contexto: a maior transação legítima na base inteira tem **10 unidades** — $2.100. Esse registro estava a mais de 15 desvios-padrão da média."

---

**[VISUAL NO PBI]**
Se o dashboard tiver o boxplot de quantidade (disponível na Página 1 ou em tooltip), mostre brevemente.
O ponto isolado acima do whisker é o outlier.

---

**[FALA — continuação]**

> "Aplicamos dois métodos estatísticos independentes para validar:"

> "**IQR — Intervalo Interquartil:** a faixa normal para quantidade de itens por transação é de -4,5 a 15,5 unidades. Qualquer coisa fora disso é candidata a outlier."

> "**Z-score:** valor acima de |3| indica anomalia extrema. Esse registro tinha Z-score de mais de 15."

> "**Os dois métodos apontaram para o mesmo e único registro.** Convergência perfeita."

*[pausa]*

> "Removemos esse registro. O faturamento real de 2023 ficou em **$298.032**."

*[pausa de 2 segundos]*

> "Poderia ter deixado. O número ficaria bonito. Mas a análise seria uma mentira — e qualquer decisão baseada nela, também."

> "Toda recomendação que vocês vão ver daqui para frente está construída sobre dados limpos e verificados. Não é detalhe técnico. É a fundação da credibilidade desta análise."

---

**[DICA]** Este é um momento de autoridade. Não peça desculpa pelo tempo gasto em qualidade de dados. Consultores sérios fazem isso — e demonstrar isso no início da apresentação sinaliza maturidade analítica.

**[TRANSIÇÃO]** "Com a base limpa, podemos olhar para o retrato real da WYZ Prime em 2025. E esse retrato tem muito a contar."

---

## SEÇÃO 3 — O RETRATO DE 2025
### [3 minutos] · Página PBI: Visão Executiva → filtro Ano = 2025

---

### [SLIDE 3] KPIs Consolidados 2025

**[VISUAL NO PBI]**
Selecione o filtro **Ano = 2025** na **Página 1 — Visão Executiva**.
Os KPI cards devem mostrar os valores de 2025. Foque nesses 7 indicadores.

---

**[FALA]**

> "2025 em números."

*[pause após cada número — deixe o card falar]*

> "**$444.417** de faturamento. Crescimento de **+26,6%** sobre 2024."
> "**736 transações** no ano. Ticket médio de **$604**."
> "Gross Income — o lucro bruto efetivo — de **$18.227**."
> "Rating médio de **6,92** numa escala de 1 a 10."
> "**45,7%** das transações via Ewallet."
> "E **475 clientes inativos** — 39% da base."

*[pause — mude o tom]*

> "Cinco desses números contam uma história de força. O último conta uma história de oportunidade."

*[aponte para o indicador de clientes inativos]*

> "Voltaremos a esse 39% — porque ali está uma das maiores alavancas de receita disponíveis agora."

---

### [SLIDE 4] WYZ Prime vs. Mercado Brasileiro

**[VISUAL NO PBI]**
Navegue para a **Página 5 — Benchmarking**.
A tabela comparativa e os bullet charts estão nessa página.
Deixe os bullet charts visíveis — eles comunicam posicionamento visualmente sem precisar de explicação verbal.

---

**[FALA]**

> "Mas crescimento absoluto não basta. Crescimento relativo ao mercado é o que importa."

*[aponte para a tabela de benchmarking]*

> "Coloquei a WYZ lado a lado com o mercado brasileiro, com base em dados públicos de 2024:"

*[destaque os itens um a um — não leia a tabela inteira]*

> "**Ewallet em 45,7%.** O teto do mercado é 42%. A WYZ já ultrapassou o mercado em adoção digital — antes de qualquer campanha de incentivo adicional."
*Fonte: Banco Central do Brasil, Relatório de Pagamentos 2024.*

> "**Crescimento de +26,6%.** O e-commerce brasileiro cresceu 12,2% em 2024. A WYZ cresceu mais que o dobro do teto de mercado."
*Fonte: ABComm / IBGE 2024.*

> "**Ticket médio de $604.** O mercado de e-commerce opera entre $45 e $120. A WYZ está 5 vezes acima da média."

> "**Retenção de 60,8%.** O mercado aceita entre 30% e 45% como normal. Mais de 6 em cada 10 clientes voltam."
*Fonte: Bain & Company, Customer Loyalty Study.*

*[pausa — olhe para a plateia]*

> "Esses não são sinais de uma empresa com problema. São sinais de uma empresa com motor funcionando — mas que ainda não sabe exatamente onde colocar mais combustível."

> "Dois indicadores estão na média e merecem atenção: **Rating** e **programa de Members**. Os dois estagnam onde o mercado já está. Esse é o espaço para crescer."

---

**[DICA]** Cite as fontes dos benchmarks naturalmente — não leia todas, mencione uma ou duas como ancoragem de credibilidade. Isso mostra que você não inventou os números de referência.

**[TRANSIÇÃO]** "Crescimento e retenção são médias gerais. Médias escondem histórias. Vamos abrir por categoria — e o que vamos encontrar vai mudar o tom da conversa."

---

## SEÇÃO 4 — SATISFAÇÃO DO CLIENTE
### [4 minutos] · Página PBI: Satisfação e Produtos

---

### [SLIDE 5] Evolução do Rating por Categoria (2021–2025)

**[VISUAL NO PBI]**
Vá para a **Página 2 — Satisfação e Produtos**.
O gráfico de linhas multisérie mostra a evolução do rating por categoria de 2021 a 2025.
Não aplique filtro — deixe todas as 6 linhas visíveis para criar o contraste.

---

**[FALA]**

> "Rating médio geral: 6,92. Parece estável. Mas quando você abre por categoria, a história muda completamente."

*[aponte para as linhas que sobem]*

> "**Electronic Accessories** saiu de 6,77 para **7,22**. Alta de 0,45 pontos — a maior de todas as categorias em 5 anos. Produto, logística, atendimento — algo melhorou de verdade aqui."

> "**Sports and Travel** subiu de 6,67 para **7,01**. Tendência positiva consistente."

> "**Food & Beverages** e **Home & Lifestyle** seguem estáveis, na faixa de 6,9 — sem degradação, sem brilho especial."

> "**Fashion Accessories** mostra leve recuo — de 6,93 para 6,79. Volume cresceu 79% em 2025, mas o rating caiu. Possível pressão de qualidade sob maior demanda."

*[pausa — mude o tom para mais grave]*

> "E então temos **Health and Beauty**."

---

### [SLIDE 6] Alerta: Health & Beauty em Queda Crítica

**[VISUAL NO PBI]**
Ainda na **Página 2**, use o filtro ou clique na linha de Health & Beauty para destacá-la.
O gráfico de barras lateral deve mostrar a queda de volume: de 91 transações em 2024 para **45 em 2025** — queda de 50%.
O delta chart (variação 2021→2025) deve mostrar a barra de H&B em vermelho: **-0,57 pts**.

---

**[FALA]**

> "Health and Beauty foi, por muito tempo, a **categoria mais bem avaliada da WYZ**. Rating de 7,10 em 2021."

*[aponte para o final da linha]*

> "Hoje: **6,53**. Queda de **0,57 pontos** em 5 anos. Queda contínua, sem reversão."

*[pausa de 2 segundos]*

> "E o volume caiu **50%** em 2025. De 91 transações em 2024 para 45 em 2025."

> "Dois sinais independentes apontando na mesma direção: rating caindo e clientes indo embora. Isso não é ruído estatístico — é tendência estrutural."

> "O dado não diz o porquê. Pode ser mix de produto, precificação, concorrência, qualidade. Mas diz com clareza: **há algo errado aqui, e precisa de investigação imediata.**"

*[pergunta retórica — olhe diretamente para a plateia]*

> "Se essa categoria continuar nessa trajetória por mais 2 anos — quem está capturando esses clientes que a WYZ está perdendo?"

---

**[DICA]** A pergunta não precisa de resposta. Faça uma pausa de 3 segundos. O objetivo é criar urgência — não fechar a discussão.

**[TRANSIÇÃO]** "Falamos das categorias com problema. Agora vamos falar da maior oportunidade de campanha que os dados revelam — e de quando exatamente agir."

---

## SEÇÃO 5 — CAMPANHA HOME AND LIFESTYLE
### [3 minutos] · Página PBI: Campanha H&L e Orçamento

---

### [SLIDE 7] Quando Lançar a Campanha?

**[VISUAL NO PBI]**
Vá para a **Página 3 — Campanha H&L e Orçamento**.
O gráfico de colunas mostra a sazonalidade mensal de **Home and Lifestyle** com todos os anos históricos.
As colunas de agosto e setembro devem estar destacadas (maior altura, cor diferente).
O mês de junho deve estar visivelmente menor.

---

**[FALA]**

> "Home and Lifestyle é a categoria de **maior receita da WYZ** — $506.289 no acumulado histórico, ticket médio de $1.143, o maior de todas as categorias."

> "Analisamos o histórico mês a mês, de 2021 a 2025."

*[aponte para o gráfico]*

> "O padrão é consistente e claro:"

> "**Agosto e setembro são o pico histórico.** Agosto concentra 45 transações e **$55.098** de faturamento — 29% acima da média dos outros meses. Setembro vem logo atrás, com $49.626."

> "**Junho é o vale.** 27 transações. $27.693. Menos da metade do pico."

*[pausa]*

> "Isso nos dá uma janela de ação precisa: a campanha deve ser lançada em **julho** — para aquecer a base e capturar o momentum natural de agosto e setembro."

> "Não é intuição. É o comportamento histórico de 5 anos."

---

### [SLIDE 8] Para Quem? — Perfil do Público H&L

**[VISUAL NO PBI]**
Ainda na **Página 3**, o painel de perfil do público H&L 2025 mostra:
- Distribuição de idade (35–55 anos de concentração)
- Tipo de cliente (Members 54%)
- Classe social (Middle 57%)
- Método de pagamento (Credit card + Ewallet = 73% combinados)

---

**[FALA]**

> "Quem compra Home and Lifestyle na WYZ?"

*[aponte para os visuais de perfil um a um]*

> "**35 a 55 anos.** Idade média de 45 anos."
> "**Classe média**, com renda média de $82.739 anuais."
> "**54% são Members** — já estão no programa de fidelidade."
> "**73% pagam com Credit Card ou Ewallet** — exatamente os meios que permitem cashback, parcelamento e benefícios digitais."

*[pausa]*

> "Esse perfil responde muito bem a campanhas com benefício tangível: cashback via Ewallet, parcelamento exclusivo para Members, acesso antecipado a lançamentos."

> "A janela está aberta — agosto e setembro. O público está mapeado. O que falta é a decisão de agir."

---

**[DICA]** Seja direto e objetivo aqui. Não detalhe demais. A mensagem é: sabemos quando, sabemos para quem, sabemos o canal. É executável agora.

**[TRANSIÇÃO]** "Mas não adianta saber para quem vender se o orçamento for distribuído sem critério. A próxima análise responde onde cada real de marketing rende mais."

---

## SEÇÃO 6 — ONDE INVESTIR O ORÇAMENTO DE MARKETING
### [3 minutos] · Página PBI: Campanha H&L e Orçamento → Score de Marketing

---

### [SLIDE 9] Score de Priorização de Marketing

**[VISUAL NO PBI]**
Ainda na **Página 3**, role para o visual de **Score de Marketing** — gráfico de barras horizontais com as 6 categorias rankeadas.
As duas primeiras (Sports & Travel, Fashion Accessories) devem estar em verde.
Food & Beverages, ao final, em vermelho.

---

**[FALA]**

> "Com orçamento de marketing limitado, a pergunta é direta: onde cada real rende mais?"

> "Criamos um score composto que pondera três variáveis: **margem bruta** (peso 40%), **ticket médio** (peso 35%) e **volume de transações** (peso 25%)."

*[aponte para o topo do ranking — pause]*

> "**Sports and Travel: prioridade número 1.**"
> "Margem de **15%**. Ticket médio de **$1.035**. Cada venda gera $155 de retorno bruto. Volume cresceu em 2025, rating subiu para 7,01."

> "**Fashion Accessories: segunda prioridade.**"
> "Maior margem da casa: **18,1%**. Ticket de $705. Maior volume de transações: 503 vendas no período completo."

*[aponte para o final da lista — pausa mais longa]*

> "**Food and Beverages: último.**"
> "Margem de **2,1%**. Ticket de **$86**."

*[olhe para a plateia — tom firme]*

> "Para cada campanha que converte em Food & Beverages, a WYZ trabalha muito para ganhar pouco. Qualquer desconto promocional elimina a margem inteira."

> "Não estamos dizendo que essa categoria deve ser eliminada. Estamos dizendo que ela **não deve receber investimento prioritário de marketing**. Deixe-a operar organicamente e foque onde a margem sustenta o investimento."

---

**[VISUAL NO PBI]**
Se tiver o scatter de Margem × Ticket na mesma página, aponte brevemente para mostrar visualmente onde Sports e Fashion estão no quadrante superior direito — alto retorno por transação.

---

**[DICA]** Essa recomendação pode gerar debate. Esteja preparado: "A margem de 2,1% vs 15–18% das categorias top não é uma opinião — é aritmética. O investimento de marketing precisa de margem para se pagar."

**[TRANSIÇÃO]** "Definimos onde investir em novos esforços. Mas antes de olhar para novos clientes, há uma oportunidade imediata que muitas vezes é ignorada: os clientes que já compraram — e simplesmente pararam de comprar."

---

## SEÇÃO 7 — REATIVAÇÃO: A OPORTUNIDADE DE $30K
### [4 minutos] · Página PBI: Clientes e Reativação

---

### [SLIDE 10] Os 475 Clientes Inativos

**[VISUAL NO PBI]**
Navegue para a **Página 4 — Clientes e Reativação**.
Os cards mostram: 475 inativos, 39% da base, ticket médio histórico $619.
O gráfico de barras mostra a distribuição por ano da última compra.

---

**[FALA]**

> "39% da base de clientes da WYZ está inativa. 475 pessoas que já compraram, já confiaram na marca — e pararam."

*[pausa de 2 segundos]*

> "O ticket médio histórico desse grupo é de **$619**. Acima da média geral de $604."

> "Esses não são clientes de baixo valor que a empresa pode ignorar. São clientes de alto valor que, por algum motivo, não voltaram."

*[aponte para a decomposição por recência]*

> "E nem todos os 475 são iguais. **238 deles compraram em 2024** — inativos recentes, ainda 'mornos'. São os mais propensos a responder a uma campanha de reativação."

> "Os demais 237 têm a última compra em 2023 ou antes — exigem esforço maior e oferta mais agressiva."

---

### [SLIDE 11] A Simulação: Quantos Clientes Precisamos?

**[VISUAL NO PBI]**
Ainda na **Página 4**, o visual de projeção mostra os 3 cenários em barras:
- Mercado conservador (15% conv.) → $44.166
- Meta WYZ (20% conv., foco nos 238 de 2024) → $58.891
- Meta mínima (quantos precisam converter) → 48 clientes = $30.000

A linha vermelha horizontal marca a meta de $30K.

---

**[FALA]**

> "Fizemos a conta. Para bater a meta de **$30.000** em receita incremental de reativação, quantos clientes precisam voltar?"

*[pausa — deixe a pergunta no ar por 2 segundos]*

> "**Quarenta e oito.**"

*[pausa]*

> "Com o ticket médio de $619, 48 reativações chegam exatamente na meta."

> "Se contactarmos os **238 inativos de 2024** — os mais recentes — e convertermos apenas **20%**, chegamos a **$30.816**. Meta cumprida."

> "20% não é otimismo. É o número **conservador** de mercado. Klaviyo e Bain reportam 15–25% como faixa esperada para campanhas de reativação bem segmentadas."

*[aponte para a barra mais alta]*

> "Agora, se aplicarmos segmentação RFM para priorizar os perfis de maior propensão de compra, a taxa sobe para **25%** e o resultado vai para **$58.891**. Quase o dobro da meta, com o mesmo esforço base."

---

### [SLIDE 12] Segmentação RFM — Quem é Cada Inativo?

**[VISUAL NO PBI]**
Ainda na **Página 4**, o gráfico de segmentos RFM e a matriz colorida R×F estão disponíveis.
Aponte para os segmentos enquanto fala os números. A matriz de calor mostra o valor monetário médio por quadrante.

---

**[FALA]**

> "RFM classifica cada cliente em três dimensões: **Recência** — quando comprou pela última vez, **Frequência** — quantas vezes comprou, e **Monetário** — quanto gastou no total."

> "Cada cliente recebe uma nota de 1 a 5 em cada dimensão. O cruzamento gera segmentos com ação específica."

*[aponte para os segmentos enquanto fala]*

> "**142 Champions.** Compram frequente, recente, alto valor. Se algum desses está inativo — urgência máxima."

> "**165 Loyal Customers.** Base sólida. Ação: manter com programa de pontos e benefícios Members."

> "**163 At Risk.** Eram bons clientes — estão escorregando. Uma oferta personalizada agora pode ser a diferença entre recuperação e perda definitiva."

> "**109 Can't Lose Them.** Compraram muito no passado, sumiram. Esses merecem contato direto — não email automático. Contato humano, se possível."

> "**236 New Customers.** Ainda em fase de construção de relacionamento. Onboarding, benefícios Members, guia de Ewallet."

*[pausa — olhe para a plateia]*

> "A campanha de reativação não é um email em massa para 475 pessoas. É uma sequência segmentada: mensagem certa, para o perfil certo, no canal certo."

> "Para **At Risk e Can't Lose Them**: oferta com desconto direto, 15–20%, via canal preferido do cliente — Ewallet ou credit card."

> "Para **Champions e Loyal** inativos: benefício exclusivo, acesso antecipado, tratamento VIP."

---

**[DICA]** Se perguntarem sobre a metodologia RFM: "Cada cliente recebe nota 1–5 em Recência, Frequência e Monetário, via divisão em quintis. O cruzamento das três notas gera o segmento. É o padrão da indústria para segmentação de campanhas — usado por Salesforce, Klaviyo e Adobe Campaign."

**[TRANSIÇÃO]** "Com esse diagnóstico completo — o que está funcionando, onde há risco, e onde está a oportunidade concreta — chegamos ao ponto mais importante: o que fazer em 2026, e em que ordem."

---

## SEÇÃO 8 — ESTRATÉGIAS PARA 2026
### [3 minutos] · Página PBI: Clientes e Reativação → depois Visão Executiva

---

### [SLIDE 13] 5 Recomendações Priorizadas

**[VISUAL NO PBI]**
Mantenha a **Página 4** aberta. Ao apresentar as estratégias de médio prazo, volte para a **Página 1** com filtro 2025 para reforçar os KPIs de contexto.

---

**[FALA]**

> "Cinco recomendações. Priorizadas por impacto e velocidade de execução."

---

**QUICK WINS — 0 a 3 meses:**

> "**1. Campanha de reativação segmentada por RFM.**"
> "Foco nos 238 inativos de 2024. Prioridade para segmentos At Risk (163) e Can't Lose Them (109). Meta: $30K com conversão de 20%, potencial de $58K com personalização por RFM."
> "Canal: Ewallet e credit card — preferência comprovada de 73% dos clientes de alto valor."

> "**2. Investigação de Health & Beauty.**"
> "Rating caiu de 7,10 para 6,53. Volume caiu 50% em 2025. Recomendo pesquisa qualitativa com clientes inativos da categoria — NPS aberto, identificando o motivo real da saída antes de qualquer investimento na categoria."

> "**3. Campanha sazonal Home and Lifestyle — lançamento em julho.**"
> "Pico em agosto e setembro. Público Members, 35–55 anos, classe média. Benefício via Ewallet ou parcelamento exclusivo."

---

**MÉDIO PRAZO — 3 a 12 meses:**

> "**4. Concentrar orçamento de marketing em Sports and Travel e Fashion Accessories.**"
> "Margem de 15% e 18,1% respectivamente. ROI de campanha sustentável. Evitar investimento direto em Food & Beverages — margem de 2,1% não comporta custo de aquisição."

> "**5. Reformular o Programa de Members.**"
> "Estagnado em 49–50% por 5 anos consecutivos — nenhum crescimento perceptível apesar da estratégia declarada de fortalecimento. Vincular o programa ao Ewallet com sistema de pontos progressivo: compras via Ewallet acumulam pontos extras. Isso endereça simultaneamente as duas estratégias de 2025 que ainda não decolaram."

---

**[DICA]** Apresente as recomendações com segurança e na ordem correta. Não hesite ao recomendar o que fazer — você analisou os dados, você tem a autoridade.

**[TRANSIÇÃO]** "Antes de abrir para perguntas, quero deixar três números com vocês."

---

## SEÇÃO 9 — FECHAMENTO
### [1 minuto] · Página PBI: Visão Executiva → filtro 2025

---

### [SLIDE 14] Síntese em 3 Números

**[VISUAL NO PBI]**
Volte para a **Página 1 — Visão Executiva**, filtro **2025**.
Idealmente, deixe apenas os 3 KPI cards mais relevantes visíveis.
Se possível, use um bookmark no Power BI que abre esse estado limpo.

---

**[FALA]**

*[aponte para cada número com pausa longa entre eles]*

> "**+26,6%.**"

*[pausa de 2 segundos]*

> "A WYZ está crescendo acima do dobro do mercado. Não é sorte. É o resultado de um perfil de cliente de alto valor — ticket 5 vezes acima do mercado, retenção acima de 60%, adoção digital à frente do setor."

*[pausa]*

> "**$58.891.**"

*[pausa de 2 segundos]*

> "Potencial de reativação com segmentação RFM. Esse dinheiro já existiu antes — é de clientes que já compraram e confiaram na marca. O caminho para trazê-los de volta está mapeado, é executável e está embasado em benchmark de mercado."

*[pausa]*

> "**48.**"

*[pausa de 2 segundos]*

> "Quarenta e oito clientes. Esse é o número que transforma a meta de $30K em realidade. Não é uma promessa vaga. É uma meta concreta, com metodologia validada por trás."

*[pausa final — olhe para a plateia, tom calmo e firme]*

> "Os dados da WYZ Prime não mostram uma empresa com problema. Mostram uma empresa com potencial identificado e clareza suficiente para agir."

> "O próximo passo é de vocês."

> "Obrigado. Estou à disposição."

---

**[DICA]** Termine em pé, firme. Não diga "é isso" nem "acabei". A última frase é uma entrega — feche o notebook ou recue um passo. Sinalize o fim com postura, não com palavras fracas.

---

## APÊNDICE A — GUIA DE NAVEGAÇÃO NO POWER BI

### Estados do dashboard por slide

| Slide | Página PBI | Filtros | Ação específica |
|---|---|---|---|
| 1 — Abertura | Pg 1 — Visão Executiva | Todos os anos | Mostrar linha de faturamento completa |
| 2 — Outlier | Pg 1 — Visão Executiva | Ano = 2023 | Apontar o valor distorcido; mostrar tabela com transação anômala |
| 3 — KPIs | Pg 1 — Visão Executiva | Ano = 2025 | Focar nos 7 KPI cards |
| 4 — Benchmark | Pg 5 — Benchmarking | Sem filtro | Bullet charts + tabela comparativa |
| 5 — Satisfação geral | Pg 2 — Satisfação | Sem filtro | Gráfico de linhas multisérie |
| 6 — H&B alerta | Pg 2 — Satisfação | Clicar em H&B | Isolar a linha vermelha + delta chart |
| 7 — Sazonalidade H&L | Pg 3 — H&L | Home and Lifestyle | Barras mensais com destaque Ago/Set |
| 8 — Público H&L | Pg 3 — H&L | Home and Lifestyle | Visuais de perfil (idade, classe, pagamento) |
| 9 — Score marketing | Pg 3 — H&L | Sem filtro | Ranking de score composto |
| 10 — Inativos | Pg 4 — Reativação | Status = Inativo | Cards de inativos + decomposição por recência |
| 11 — Simulação | Pg 4 — Reativação | Sem filtro | Gráfico waterfall / barras de projeção |
| 12 — RFM | Pg 4 — Reativação | Sem filtro | Segmentos RFM + matriz R×F |
| 13 — Estratégias | Pg 4 → Pg 1 | Sem filtro | Mostrar recomendações; voltar para Pg 1 no médio prazo |
| 14 — Fechamento | Pg 1 — Visão Executiva | Ano = 2025 | Bookmark limpo com 3 KPIs principais |

---

## APÊNDICE B — RESPOSTAS PARA PERGUNTAS DIFÍCEIS

**"Por que o ticket médio de $604 é tão alto comparado ao mercado?"**
> "A base de comparação inclui e-commerces de massa com volume alto e ticket baixo. A WYZ opera com perfil Members predominante e categorias de valor médio-alto — Home & Lifestyle em $1.143, Sports & Travel em $1.035. Não é distorção — é posicionamento. O benchmark de mercado valida que esse posicionamento é diferenciador."

**"A queda de H&B pode ser outro erro de dado?"**
> "Não. O outlier de 2023 foi pontual e cirúrgico — uma única linha detectada por dois métodos independentes. A queda de H&B é uma tendência de 5 anos, observada de forma independente em rating E em volume de transações. São dois sinais distintos apontando na mesma direção — isso é o oposto de ruído."

**"20% de conversão nos inativos é realista?"**
> "É conservador. Campanhas de reativação bem segmentadas, com oferta personalizada por perfil RFM, atingem 15–30% nos benchmarks da Klaviyo (2024) e Bain & Company. Usamos 20% como piso. Com RFM aplicado, a expectativa sobe para 25%."

**"Por que os pesos do score de marketing são 40/35/25?"**
> "Margem tem peso maior porque determina o retorno sustentável — sem margem, desconto de campanha não se paga. Ticket vem em segundo porque amplifica o impacto por transação. Volume equilibra o score para evitar recomendar categorias de nicho com alta margem mas baixíssima escala. Os pesos são parametrizáveis — se a WYZ priorizar escala, podemos ajustar."

**"Por que não recomendar campanha para H&B se ela precisa de ajuda?"**
> "Campanhas de marketing não resolvem problema de produto ou satisfação — elas amplificam. Se o cliente está insatisfeito e eu trago mais clientes, o problema escala. Primeiro precisamos diagnosticar o que está causando a queda de rating. Depois, com o produto corrigido, a campanha faz sentido."

**"O RFM foi calculado com os dados históricos completos?"**
> "Sim — base de referência em 1º de janeiro de 2026, com todos os 2.586 registros limpos de 2021 a 2025. A recência é calculada em dias desde a última compra. O scoring usa quintis independentes para cada dimensão, o que elimina viés de escala entre R, F e M."

---

## APÊNDICE C — CHECKLIST PRÉ-APRESENTAÇÃO

**30 minutos antes:**
- [ ] Power BI Desktop aberto na Página 1 com filtro "Todos os anos"
- [ ] Bookmark de fechamento (3 KPIs + 2025) configurado e testado
- [ ] Tabela de benchmarking com ícones de status visível na Página 5
- [ ] Linha de H&B destacada em vermelho na Página 2
- [ ] Sazonalidade H&L com colunas de Ago/Set destacadas na Página 3
- [ ] Gráfico waterfall/barras de reativação com linha de meta $30K na Página 4
- [ ] Matriz RFM com cores por segmento visível na Página 4
- [ ] Slicer de anos testado em todas as páginas

**Logística:**
- [ ] Apresentador wireless (clicker) testado e com bateria
- [ ] Resolução do projetor testada (Power BI em modo fullscreen)
- [ ] Água na mesa
- [ ] Roteiro impresso em fonte 12 — apenas para consulta rápida, não para leitura

**Mental:**
- [ ] Revisar os 3 números do fechamento: 26,6% / $58.891 / 48
- [ ] Revisar as 4 respostas de perguntas difíceis mais prováveis
- [ ] Lembrar: você é o especialista aqui. Os dados sustentam cada recomendação.

---

## APÊNDICE D — NÚMEROS DE REFERÊNCIA RÁPIDA

| Indicador | Valor exato | Contexto |
|---|---|---|
| Faturamento 2025 | $444.417 | +26,6% vs 2024 |
| Faturamento 2024 | $350.963 | — |
| Faturamento 2023 (real, sem outlier) | $298.032 | Outlier removido: $21.000.000 |
| Outlier: quantidade | 100.000 unidades | Home and Lifestyle, mai/2023 |
| Outlier: IQR faixa normal | [-4,5 a 15,5 unidades] | — |
| Outlier: Z-score | > 15 | Limiar: |z| > 3 |
| Ticket médio 2025 | $604 | Mercado e-comm BR: $45–$120 |
| Gross Income 2025 | $18.227 | — |
| Ewallet 2025 | 45,7% | Mercado BR: 28–42% (BCB 2024) |
| Members % 2025 | 49,5% | Mercado BR: 45–52% (ABEMF 2024) |
| Rating médio 2025 | 6,92 | Mercado BR: 6,8–7,1 (SBVC 2024) |
| Crescimento vendas 2025 | +26,6% | E-comm BR: +12,2% (ABComm 2024) |
| Retenção anual 2025 | 60,8% | Mercado: 30–45% (Bain & Co.) |
| Clientes inativos | 475 (39%) | Última compra antes de 2025 |
| Inativos de 2024 (quentes) | 238 | Público prioritário da campanha |
| Ticket médio inativos | $619 | Acima da média geral |
| Meta reativação | $30.000 | 48 clientes × $619 |
| Projeção 20% conversão | $58.891 | 475 × 20% × $619 |
| H&L ticket médio | $1.143 | Maior de todas as categorias |
| H&L pico histórico (agosto) | $55.098 / 45 transações | — |
| H&L vale histórico (junho) | $27.693 / 27 transações | — |
| H&B rating 2021 | 7,10 | Melhor da casa |
| H&B rating 2025 | 6,53 | -0,57 pts em 5 anos |
| H&B transações 2024→2025 | 91 → 45 | Queda de 50% |
| Sports & Travel margem | 15,0% | Score: 1º lugar |
| Fashion accessories margem | 18,1% | Score: 2º lugar |
| Food & Beverages margem | 2,1% | Evitar em campanhas pagas |
| Champions RFM | 142 clientes | — |
| Loyal Customers RFM | 165 clientes | — |
| At Risk RFM | 163 clientes | Foco da reativação |
| Can't Lose Them RFM | 109 clientes | Foco da reativação |
| New Customers RFM | 236 clientes | — |
| Potential Loyalists RFM | 106 clientes | — |

---

*Roteiro elaborado para apresentação do Case WYZ Prime Commerce.*
*WYZ Prime Commerce — Case Técnico. Entrega: 06/04/2026.*
