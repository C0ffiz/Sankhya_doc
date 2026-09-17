# Tela Análise de Receitas

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/41305132391191-Tela-An%C3%A1lise-de-Receitas](https://ajuda.sankhya.com.br/hc/pt-br/articles/41305132391191-Tela-An%C3%A1lise-de-Receitas)

---

# Tela Análise de Receitas

Módulo: Financeiro  
Caminho de acesso: Menu Principal › Sankhya Finance › Análise de Receitas

Esta tela está disponível exclusivamente para clientes Sankhya Cloud.

**Neste artigo**

*   [O que é e para que serve](#oque)
*   [Filtros disponíveis](#filtros)
*   [Comportamento da tela](#comportamento)
*   [Indicadores](#indicadores)
*   [Receita mensal e média acumulada](#mensal)
*   [Receita por natureza](#natureza)
*   [Receitas por parceiro](#parceiro)
*   [Insights do período](#insights)
*   [Detalhamento ao clicar nos gráficos](#detalhamento)
*   [Extrato de Transações](#extrato)
*   [Pontos de atenção](#pontos)

## O que é e para que serve

A **Tela Análise de Receitas** reúne indicadores, gráficos e extrato das entradas financeiras — vendas, serviços, aluguéis e demais receitas. Todos os componentes respondem ao mesmo conjunto de filtros e se atualizam juntos. Use-a para entender de onde vem a receita, como ela se distribui entre naturezas e parceiros, e como se comporta ao longo dos meses. A tela é de consulta: não realiza lançamentos nem permite editar títulos.

![home receitas .png](https://ajuda.sankhya.com.br/hc/article_attachments/43504245656087)

---

## Filtros disponíveis

Os filtros controlam todos os indicadores, gráficos e o extrato ao mesmo tempo. O indicador numérico ao lado do ícone de filtro mostra quantos estão ativos.

<table style="border-collapse: collapse;"><tbody><tr><td style="border-color: #999; padding: 6px;"><strong>Filtro</strong></td><td style="border-color: #999; padding: 6px;"><strong>O que faz</strong></td></tr><tr><td style="border-color: #999; padding: 6px;"><strong>Caixa</strong> / <strong>Competência</strong></td><td style="border-color: #999; padding: 6px;">Define se as provisões entram na análise</td></tr><tr><td style="border-color: #999; padding: 6px;"><strong>Empresa</strong></td><td style="border-color: #999; padding: 6px;">Restringe às empresas selecionadas. Em branco, considera todas as que o seu usuário pode ver</td></tr><tr><td style="border-color: #999; padding: 6px;"><strong>Data de negociação</strong></td><td style="border-color: #999; padding: 6px;">Intervalo pela data em que o título foi negociado</td></tr><tr><td style="border-color: #999; padding: 6px;"><strong>Data de vencimento</strong></td><td style="border-color: #999; padding: 6px;">Intervalo pela data de vencimento</td></tr><tr><td style="border-color: #999; padding: 6px;"><strong>Data da baixa</strong></td><td style="border-color: #999; padding: 6px;">Intervalo pela data em que o título foi recebido</td></tr><tr><td style="border-color: #999; padding: 6px;"><strong>Centro de resultado</strong></td><td style="border-color: #999; padding: 6px;">Restringe por centro de resultado, considerando o rateio do título</td></tr><tr><td style="border-color: #999; padding: 6px;"><strong>Natureza</strong></td><td style="border-color: #999; padding: 6px;">Restringe por natureza, considerando o rateio do título</td></tr></tbody></table>

Os três filtros de data funcionam de forma independente e podem ser combinados.

**ℹ️ Nota**

O alternador **Caixa** / **Competência** não muda a data usada na análise. Em Caixa, a tela considera apenas títulos reais. Em Competência, considera títulos reais e provisões. A distribuição mensal continua sendo feita pela data de negociação nos dois casos.

[↑ Voltar ao início](#sumario)

---

## Comportamento da tela

<table style="border-collapse: collapse;"><tbody><tr><td style="border-color: #999; padding: 6px;"><strong>Situação</strong></td><td style="border-color: #999; padding: 6px;"><strong>O que acontece</strong></td></tr><tr><td style="border-color: #999; padding: 6px;">Abrindo ou mudando os filtros</td><td style="border-color: #999; padding: 6px;">A tela exibe uma animação enquanto carrega</td></tr><tr><td style="border-color: #999; padding: 6px;">Voltando sem mudar os filtros</td><td style="border-color: #999; padding: 6px;">A exibição é imediata, sem recarregar</td></tr><tr><td style="border-color: #999; padding: 6px;">Sem lançamentos no período</td><td style="border-color: #999; padding: 6px;">A tela exibe uma mensagem de ausência de dados</td></tr><tr><td style="border-color: #999; padding: 6px;">Erro de conexão</td><td style="border-color: #999; padding: 6px;">A tela exibe uma mensagem com o botão <strong>Tentar novamente</strong></td></tr></tbody></table>

[↑ Voltar ao início](#sumario)

---

## Indicadores

Quatro cards resumem a posição de receitas no período filtrado. Cada um exibe a variação percentual em relação ao período anterior, em verde quando favorável e em vermelho quando desfavorável.![Indicadores · 09/2026](https://ajuda.sankhya.com.br/hc/article_attachments/43504245657367)

<table style="border-collapse: collapse;"><tbody><tr><td style="border-color: #999; padding: 6px;"><strong>Indicador</strong></td><td style="border-color: #999; padding: 6px;"><strong>Como é calculado</strong></td></tr><tr><td style="border-color: #999; padding: 6px;">Receita Total</td><td style="border-color: #999; padding: 6px;">Soma do valor líquido dos títulos de receita do período, aplicando o percentual de rateio de cada título</td></tr><tr><td style="border-color: #999; padding: 6px;">Média Mensal</td><td style="border-color: #999; padding: 6px;">Receita Total dividida pela quantidade de meses com movimento no período. Mês sem título não entra no divisor</td></tr><tr><td style="border-color: #999; padding: 6px;">Média de Parceiros</td><td style="border-color: #999; padding: 6px;">Quantidade de parceiros distintos com receita no período</td></tr><tr><td style="border-color: #999; padding: 6px;">Ticket Médio</td><td style="border-color: #999; padding: 6px;">Receita Total dividida pela quantidade de parceiros distintos</td></tr></tbody></table>

**ℹ️ Nota**

O **Ticket Médio** é por parceiro, não por título. Ele responde "quanto cada parceiro representa em média", e não "quanto vale em média um título".

[↑ Voltar ao início](#sumario)

---

## Receita mensal e média acumulada

Mostra a receita de cada mês em barras, com a linha da média acumulada sobreposta.

![Receita mensal e média acumulada · 09/2026](https://ajuda.sankhya.com.br/hc/article_attachments/43504198624023)

*   Barras — receita do mês.
*   Linha — média acumulada até aquele mês.

Barra acima da linha indica mês acima da própria média histórica da empresa. Use o gráfico para identificar sazonalidade e acompanhar a tendência ao longo do ano.

Os meses são formados pela data de negociação do título.

Clique em uma barra para abrir o detalhamento com os títulos que compõem aquele mês.

[↑ Voltar ao início](#sumario)

---

## Receita por natureza

Mostra como a receita se distribui entre as naturezas financeiras.

![Receita por natureza · 09/2026](https://ajuda.sankhya.com.br/hc/article_attachments/43504245658775)

O gráfico tem dois modos, selecionados pelo alternador no canto superior direito:

*   **Total** — soma da receita de cada natureza no período.
*   **Média** — receita média mensal de cada natureza, ou seja, o total da natureza dividido pela quantidade de meses em que ela teve movimento.

Comparar os dois modos separa a natureza que soma muito por volume de títulos daquela que soma muito por poucos títulos de valor alto.

Use **Ver mais** para exibir as naturezas que não couberam no gráfico.

**ℹ️ Nota**

O rateio é considerado: título sem rateio entra integralmente na natureza informada nele, e título rateado é distribuído entre as naturezas do rateio, na proporção de cada uma.

Clique em uma barra para abrir o detalhamento com os títulos daquela natureza.

[↑ Voltar ao início](#sumario)

---

## Receitas por parceiro

Mostra os parceiros com maior volume de receita no período, em barras horizontais, do maior para o menor.

![Receitas por parceiro · 09/2026](https://ajuda.sankhya.com.br/hc/article_attachments/43504245660567)

Use o gráfico para avaliar concentração de carteira. Barra muito maior que as demais indica dependência de um parceiro.

O valor de cada parceiro considera o percentual de rateio dos títulos.

Clique em uma barra para abrir o detalhamento com os títulos daquele parceiro.

[↑ Voltar ao início](#sumario)

---

## Insights do período

Painel com leituras automáticas do recorte filtrado. A tela exibe até três insights por vez, selecionados conforme a situação dos dados.

![Insights do período · 09/2026](https://ajuda.sankhya.com.br/hc/article_attachments/43504198628503)

Exemplos de insight exibidos nesta tela:

<table style="border-collapse: collapse;"><tbody><tr><td style="border-color: #999; padding: 6px;"><strong>Insight</strong></td><td style="border-color: #999; padding: 6px;"><strong>O que informa</strong></td></tr><tr><td style="border-color: #999; padding: 6px;">Provisão anual</td><td style="border-color: #999; padding: 6px;">Valor de receitas provisionadas para o ano</td></tr><tr><td style="border-color: #999; padding: 6px;">Receitas a receber hoje</td><td style="border-color: #999; padding: 6px;">Valor a receber com vencimento no dia, e quanto já foi recebido</td></tr><tr><td style="border-color: #999; padding: 6px;">Concentração de clientes</td><td style="border-color: #999; padding: 6px;">Quantidade de parceiros que compraram no mês de referência, comparada com a média dos últimos doze meses</td></tr></tbody></table>

Os insights respeitam o filtro de empresa e têm janela própria de tempo — eles não seguem o filtro de período da tela.

[↑ Voltar ao início](#sumario)

---

## Detalhamento ao clicar nos gráficos

Clicar em uma barra dos gráficos abre uma janela com o recorte correspondente:

*   Quantidade de títulos no contexto clicado
*   Valor total do contexto
*   Lista dos títulos, com número, empresa, parceiro, natureza, data de negociação, data de vencimento, valor e situação

[↑ Voltar ao início](#sumario)

---

## Extrato de Transações

Lista paginada com todos os títulos de receita do período filtrado. Navegar entre as páginas não recarrega os gráficos.

![Extrato de Transações · 09/2026](https://ajuda.sankhya.com.br/hc/article_attachments/43504245661719)

Colunas disponíveis: Nº Financeiro, Código do parceiro, Parceiro, Natureza, Data de negociação, Vencimento, Baixa, Valor do desdobramento, Valor da baixa, Valor líquido, Provisão e Situação.

Use a barra de rolagem horizontal para alcançar as colunas à direita. O cabeçalho do extrato exibe a faixa de registros e o total encontrado.

### Situação do título

A coluna **Situação** apresenta um status por título, avaliado nesta ordem de precedência:

1.  Antecipado
2.  Renegociado
3.  Compensado
4.  Baixa parcial
5.  Baixado
6.  Vencido
7.  Aberto

[↑ Voltar ao início](#sumario)

---

## Pontos de atenção

*   Caixa e Competência não mudam a data: o alternador decide apenas se as provisões entram. A distribuição mensal segue sempre a data de negociação.
*   Média Mensal ignora meses sem movimento: o divisor é a quantidade de meses que tiveram título, não a quantidade de meses do período. Em um recorte de doze meses com movimento em oito, o divisor é oito.
*   O rateio é considerado em todos os números: título rateado entra proporcionalmente nos indicadores, nos gráficos e no extrato.
*   Os filtros são zerados ao trocar de tela: ao ir de Análise de Receitas para Análise de Despesas, refaça a seleção.
*   O valor considerado em toda a tela é o valor líquido do título. Quando o título não tem valor líquido apurado, a tela usa o valor do desdobramento.