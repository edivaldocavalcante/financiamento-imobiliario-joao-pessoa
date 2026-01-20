Fontes de Dados e Métodos de Coleta
1. Contextualização

Este projeto tem como objetivo analisar a evolução do crédito imobiliário destinado a pessoas físicas no Brasil, com foco interpretativo no contexto do município de João Pessoa (PB). Para isso, foram utilizadas exclusivamente fontes públicas, oficiais e não confidenciais, garantindo a reprodutibilidade e a transparência da análise.

Durante a fase de levantamento de dados, diferentes bases públicas foram avaliadas, considerando critérios como atualização temporal, granularidade, confiabilidade e aderência ao problema proposto.

2. Fonte de Dados Utilizada — Banco Central do Brasil (BACEN)
2.1 Descrição da fonte

A principal fonte de dados utilizada neste estudo foi o Banco Central do Brasil (BACEN), por meio do Sistema Gerenciador de Séries Temporais (SGS).

O BACEN disponibiliza séries temporais oficiais relacionadas ao sistema financeiro nacional, incluindo dados sobre concessões de crédito imobiliário, segmentados por tipo de tomador (pessoas físicas e jurídicas).

2.2 Conjunto de dados selecionado

Foi selecionada a série:

Concessões de crédito com recursos direcionados – Pessoas físicas – Financiamento imobiliário total

Unidade: R$ (milhões)

Periodicidade: Mensal

Período analisado: 2015 a 2025

Essa série representa o volume mensal de crédito imobiliário concedido a pessoas físicas no Brasil, sendo altamente relevante para compreender a dinâmica do mercado habitacional e o acesso ao financiamento ao longo do tempo.

2.3 Tipo de dados

Estruturados

Formato original: tabela/série temporal

Granularidade: mensal

Escala: valores agregados nacionais

2.4 Método de coleta

A coleta dos dados foi realizada por meio de:

Download direto da série temporal no portal do BACEN (SGS)

Exportação em formato CSV

Posterior tratamento e padronização em Google Sheets e Python

Após o download, os dados passaram por etapas de:

Padronização do formato de data (YYYY-MM)

Garantia de consistência numérica

Remoção de valores nulos

Versionamento do arquivo tratado no repositório do projeto

O arquivo final utilizado na análise encontra-se em:

data/raw/bacen_concessoes_financiamento_imobiliario_pf_tratado.csv

3. Fonte Avaliada e Não Utilizada — IBGE (PNAD Contínua / SIDRA)
3.1 Avaliação inicial

O Instituto Brasileiro de Geografia e Estatística (IBGE), por meio da PNAD Contínua (SIDRA), foi inicialmente avaliado como possível fonte para complementar a análise, especialmente para indicadores de renda domiciliar e classes de rendimento.

3.2 Limitações identificadas

Após análise técnica, a base do IBGE foi descartada para este projeto, pelos seguintes motivos:

As tabelas de renda domiciliar mais relevantes apresentavam dados desatualizados, com último período disponível em 2005–2006

Ausência de granularidade adequada para o município de João Pessoa (PB) em séries temporais longas

Incompatibilidade temporal com o período principal do estudo (2015–2025)

3.3 Justificativa do descarte

Dado que o objetivo do projeto é analisar tendências recentes do crédito imobiliário, o uso de dados defasados poderia comprometer a validade analítica e a interpretação dos resultados. Assim, optou-se por não incorporar dados do IBGE, mantendo a coerência temporal e metodológica do estudo.

4. Justificativa da Escolha Final da Fonte

A escolha do BACEN como fonte principal se justifica por:

Atualização frequente e confiável

Aderência direta ao tema de crédito imobiliário

Dados oficiais amplamente utilizados em análises econômicas

Estrutura adequada para análises de séries temporais

Compatibilidade com ferramentas analíticas como Python e Looker Studio

Embora os dados sejam agregados em nível nacional, eles fornecem uma base sólida para leituras mercadológicas e inferências regionais, especialmente quando combinadas com análise contextual, como no caso de João Pessoa (PB).

5. Considerações Finais

O uso consciente e criterioso de dados públicos é fundamental para análises responsáveis e replicáveis. Neste projeto, a seleção das fontes priorizou qualidade, atualidade e relevância analítica, garantindo que os insights obtidos estejam alinhados com a problemática proposta e com as exigências do projeto de parceria Semantix / EBAC.
