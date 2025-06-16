# AnaliseCrisede2008
Analise de Dados sobre a crise de 2008
# Análise de Indicadores Macroeconômicos e do Mercado Imobiliário - Crise de 2008

## Visão Geral do Projeto

Este projeto tem como objetivo principal explorar e analisar dados históricos de indicadores econômicos e do mercado imobiliário dos Estados Unidos, abrangendo o período de 1998 a 2009. A análise busca identificar tendências, correlações e, mais crucialmente, os sinais de alerta que precederam e se manifestaram durante a crise financeira global de 2008, conhecida pela bolha imobiliária e a crise do subprime.

Utilizando ferramentas de visualização de dados, o projeto desmistifica a complexidade do cenário econômico da época, transformando dados brutos em insights acionáveis que podem ilustrar os mecanismos por trás de um dos maiores colapsos financeiros da história recente.

## Dados Utilizados

Os dados utilizados nesta análise foram extraídos de um arquivo CSV (`CRISE 2008 (1).xlsx - Planilha2.csv`), contendo as seguintes séries temporais:

* **Data (IMOVEIS__date):** Período de registro dos dados.
* **IMOVEIS:** Índice de Preços de Imóveis Residenciais.
* **Juros de Hipotecas:** Taxa de Juros de Hipotecas de 30 Anos.
* **nadimplência:** Taxa de Inadimplência de Hipotecas Residenciais.
* **Estoque:** Oferta Mensal de Casas Novas para Venda.
* **Taxa Básica :** Taxa Básica de Juros (Federal Funds Rate).

## Estrutura da Análise

A análise foi estruturada em três partes principais:

### 1. Visualizações Iniciais (Gráficos Individuais)

Para cada uma das cinco séries de dados principais, foram gerados gráficos de linha que ilustram a evolução individual de cada indicador ao longo do tempo. O objetivo é fornecer uma compreensão clara das tendências de cada variável antes de combiná-las.

* **Evolução da Taxa de Inadimplência de Hipotecas Residenciais nos EUA (1998-2009)**
    * *(Série: `nadimplência`)*
* **Evolução da Taxa de Juros de Hipotecas de 30 Anos nos EUA (1998-2009)**
    * *(Série: `Juros de Hipotecas`)*
* **Evolução do Índice de Preços de Imóveis Residenciais nos EUA (1998-2009)**
    * *(Série: `IMOVEIS`)*
* **Evolução da Oferta Mensal de Casas Novas para Venda nos EUA (1998-2009)**
    * *(Série: `Estoque`)*
* **Evolução da Taxa Básica de Juros (Federal Funds Rate) nos EUA (1998-2009)**
    * *(Série: `Taxa Básica `)*

### 2. Indicadores de Alerta Combinados

Dois gráficos combinados foram criados para visualizar a interação entre pares de indicadores cruciais, permitindo a identificação de sinais de alerta mais complexos e correlacionados.

* **Indicador de Stress no Crédito Imobiliário: Inadimplência vs. Juros de Hipotecas (1998-2009)**
    * *(Séries: `nadimplência` e `Juros de Hipotecas`)*
    * **Insights:** Este gráfico revela a relação entre a dificuldade de pagamento dos mutuários e o custo do empréstimo. O principal sinal de alerta surge quando a taxa de inadimplência aumenta drasticamente, mesmo com a taxa de juros hipotecários não subindo proporcionalmente, indicando uma fragilidade subjacente e crescente na qualidade do crédito.

* **Indicador de Saturação e Desaceleração Imobiliária: Preços vs. Oferta de Casas (1998-2009)**
    * *(Séries: `IMOVEIS` e `Estoque`)*
    * **Insights:** Este gráfico mostra a dinâmica entre a valorização dos imóveis e a disponibilidade de novas construções. O ponto de alerta crítico é observado quando os preços dos imóveis começam a cair abruptamente, enquanto a oferta de novas casas, embora também em declínio, ainda se mantém em patamares elevados, sinalizando um mercado saturado e o estouro da bolha imobiliária.

### 3. Reflexão Preliminar

A análise dos indicadores combinados permite uma conclusão clara sobre os sinais que antecederam a crise de 2008. Os dados, em sua interconexão, 'gritavam' um acúmulo insustentável de fragilidades e excessos no mercado imobiliário e no sistema de crédito dos EUA. O principal 'ponto de não retorno' visualizado nos gráficos converge para o período entre meados de 2006 e 2007. Durante essa fase crítica, a combinação de uma queda acentuada nos preços dos imóveis, um excesso de oferta de casas e um aumento drástico e descontrolado da taxa de inadimplência hipotecária (descolada da trajetória das taxas de juros) revelava um cenário onde a capacidade de pagamento dos mutuários estava esgotada e o valor das garantias (os imóveis) estava em erosão, culminando em um colapso sistêmico.

## Ferramentas Utilizadas

* **Power BI Desktop:** Ferramenta de Business Intelligence para criação de dashboards e relatórios interativos.

## Como Reproduzir a Análise (no Power BI)

1.  **Carregue os dados:** Importe o arquivo `CRISE 2008 (1).xlsx - Planilha2.csv` para o Power BI Desktop.
2.  **Ajuste Tipos de Dados:** No Editor do Power Query ou na visualização de dados, garanta que a coluna `IMOVEIS__date` esteja no formato "Data" e as demais colunas numéricas (`IMOVEIS`, `Juros de Hipotecas`, `nadimplência`, `Estoque`, `Taxa Básica `) estejam como número decimal.
3.  **Crie os Gráficos Individuais:** Utilize o visual "Gráfico de Linha", colocando `IMOVEIS__date` no Eixo X (selecionando a opção de "Data" contínua, não a hierarquia) e cada uma das cinco séries (`nadimplência`, `Juros de Hipotecas`, `IMOVEIS`, `Estoque`, `Taxa Básica `) no Eixo Y, um por vez em gráficos separados.
4.  **Crie os Gráficos Combinados:**
    * **Stress no Crédito Imobiliário:** Utilize o visual "Gráfico de Linha". Coloque `IMOVEIS__date` no Eixo X, `nadimplência` no Eixo Y e `Juros de Hipotecas` no Eixo Y Secundário.
    * **Saturação e Desaceleração Imobiliária:** Utilize o visual "Gráfico de Linha". Coloque `IMOVEIS__date` no Eixo X, `IMOVEIS` no Eixo Y e `Estoque` no Eixo Y Secundário.

Para dúvidas ou mais informações, entre em contato.

---
