# Tela DRE

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/41308330140439-Tela-DRE](https://ajuda.sankhya.com.br/hc/pt-br/articles/41308330140439-Tela-DRE)

---

# Tela DRE

Módulo: Financeiro  
Caminho de acesso: Menu Principal › Sankhya Finance › DRE

Esta tela está disponível exclusivamente para clientes Sankhya Cloud.

**Neste artigo**

*   [O que é e para que serve](#oque)
*   [Pré-requisito: configurar o DRE na Contabilidade](#prereq)
*   [Estrutura do DRE](#estrutura)
*   [Filtros e barra de ferramentas](#filtros)
*   [Comportamento da tela](#comportamento)
*   [Indicadores](#indicadores)
*   [Visão Consolidado](#consolidado)
*   [Visão Mensal](#mensal)
*   [Visão Por empresa](#porempresa)
*   [Indicadores do demonstrativo](#indicadoresdemonstrativo)
*   [Pontos de atenção](#pontos)

## O que é e para que serve

A **Tela DRE** (Demonstrativo de Resultados do Exercício) apresenta a visão consolidada das receitas, despesas, custos e resultados da empresa ao longo do período analisado, organizados pela hierarquia de grupos de contas da estrutura selecionada. Use-a para acompanhar margens, comparar o realizado com o ano anterior e com o orçamento, e visualizar a composição do resultado por grupo de contas. A tela é de consulta: não realiza lançamentos nem permite editar títulos, e os valores exibidos vêm da movimentação contábil, não do módulo Financeiro.  
  
![](https://ajuda.sankhya.com.br/hc/article_attachments/43502990781975)

---

## Pré-requisito: configurar o DRE na Contabilidade

A tela não traz dados enquanto o DRE não estiver configurado no Sankhya Om. A configuração é feita na Contabilidade, em **Contabilidade › Consultas › Demonstrativos Contábeis - DRE**, e envolve:

1.  Classificar as contas no **Grupo 04 — Contas de Resultado** do plano de contas.
2.  Criar a estrutura da DRE, com grupos e subgrupos, em até cinco níveis.
3.  Fazer o **Mapeamento de Contas**, associando cada conta de resultado ao grupo correspondente da estrutura.
4.  Definir quais empresas compõem o demonstrativo.
5.  Executar **Processar DRE** para sincronizar os valores com a movimentação contábil.

Para o passo a passo completo, acesse [Demonstrativos Contábeis - DRE](https://ajuda.sankhya.com.br/hc/pt-br/articles/39229659689239-Demonstrativos-Cont%C3%A1beis-DRE).

**⚠️ Atenção**

Sem o **Processar DRE** executado depois dos lançamentos, o demonstrativo exibe os valores da última sincronização. Conta de resultado sem mapeamento não aparece em nenhum grupo, e o resultado fica incompleto sem indicar erro.

[↑ Voltar ao início](#sumario)

---

## Estrutura do DRE

Antes de carregar os dados, selecione a estrutura desejada. Cada estrutura define os grupos de contas e a hierarquia do demonstrativo, conforme configurado na Contabilidade.

A criação e a manutenção das estruturas são responsabilidade do administrador do sistema.

[↑ Voltar ao início](#sumario)

---

## Filtros e barra de ferramentas

A barra de ferramentas reúne os controles de visualização e navegação do demonstrativo:

<table style="border-collapse: collapse;"><tbody><tr><td style="border-color: #999; padding: 6px;"><strong>Controle</strong></td><td style="border-color: #999; padding: 6px;"><strong>O que faz</strong></td></tr><tr><td style="border-color: #999; padding: 6px;"><strong>Consolidado</strong> · <strong>Mensal</strong> · <strong>Por empresa</strong></td><td style="border-color: #999; padding: 6px;">Alterna entre as três visões do demonstrativo</td></tr><tr><td style="border-color: #999; padding: 6px;"><strong>Expandir</strong> / <strong>Recolher</strong></td><td style="border-color: #999; padding: 6px;">Expande ou recolhe todos os grupos de contas de uma vez</td></tr><tr><td style="border-color: #999; padding: 6px;"><strong>Exibir % RL</strong></td><td style="border-color: #999; padding: 6px;">Exibe ou oculta as colunas de percentual sobre a Receita Líquida. Disponível apenas na visão Consolidado</td></tr><tr><td style="border-color: #999; padding: 6px;"><strong>Filtros</strong></td><td style="border-color: #999; padding: 6px;">Abre os filtros adicionais, entre eles a estrutura e o período</td></tr><tr><td style="border-color: #999; padding: 6px;">(1,00) ↔ -1,00</td><td style="border-color: #999; padding: 6px;">Alterna a exibição de valores negativos entre parênteses e sinal negativo</td></tr></tbody></table>

**ℹ️ Nota**

O botão **Exibir % RL** fica indisponível nas visões Mensal e Por empresa.

[↑ Voltar ao início](#sumario)

---

## Comportamento da tela

<table style="border-collapse: collapse;"><tbody><tr><td style="border-color: #999; padding: 6px;"><strong>Situação</strong></td><td style="border-color: #999; padding: 6px;"><strong>O que acontece</strong></td></tr><tr><td style="border-color: #999; padding: 6px;">Carregando dados</td><td style="border-color: #999; padding: 6px;">A tela exibe uma animação enquanto monta o demonstrativo</td></tr><tr><td style="border-color: #999; padding: 6px;">Trocando a estrutura</td><td style="border-color: #999; padding: 6px;">Todos os dados são recarregados</td></tr><tr><td style="border-color: #999; padding: 6px;">Mudando o período</td><td style="border-color: #999; padding: 6px;">Os dados são refiltrados sem recarregar a estrutura</td></tr><tr><td style="border-color: #999; padding: 6px;">Trocando de visão</td><td style="border-color: #999; padding: 6px;">A troca é imediata, porque os dados já estão carregados</td></tr><tr><td style="border-color: #999; padding: 6px;">Sem lançamento no período</td><td style="border-color: #999; padding: 6px;">As linhas são exibidas com valores zerados</td></tr></tbody></table>

[↑ Voltar ao início](#sumario)

---

## Indicadores

Quatro cards no topo resumem o resultado do período. Cada card exibe a variação percentual em relação ao ano anterior.  
  
![Indicadores · 09/2026](https://ajuda.sankhya.com.br/hc/article_attachments/43502949476631)

<table style="border-collapse: collapse;"><tbody><tr><td style="border-color: #999; padding: 6px;"><strong>Indicador</strong></td><td style="border-color: #999; padding: 6px;"><strong>O que mostra</strong></td></tr><tr><td style="border-color: #999; padding: 6px;">Lucro Bruto</td><td style="border-color: #999; padding: 6px;">Receita líquida menos o custo das mercadorias vendidas</td></tr><tr><td style="border-color: #999; padding: 6px;">Lucro Líquido</td><td style="border-color: #999; padding: 6px;">Resultado final do período, após todas as receitas e despesas</td></tr><tr><td style="border-color: #999; padding: 6px;">EBIT</td><td style="border-color: #999; padding: 6px;">Resultado antes de juros e impostos</td></tr><tr><td style="border-color: #999; padding: 6px;">Resultado da Operação Comercial</td><td style="border-color: #999; padding: 6px;">Resultado gerado pela operação comercial no período</td></tr></tbody></table>

Os indicadores seguem a estrutura de DRE selecionada.

[↑ Voltar ao início](#sumario)

---

## Visão Consolidado

Apresenta o período inteiro em uma coluna, com as comparações lado a lado.

![Visão Consolidado · 09/2026](https://ajuda.sankhya.com.br/hc/article_attachments/43502949478551)

### Colunas

<table style="border-collapse: collapse;"><tbody><tr><td style="border-color: #999; padding: 6px;"><strong>Coluna</strong></td><td style="border-color: #999; padding: 6px;"><strong>Conteúdo</strong></td></tr><tr><td style="border-color: #999; padding: 6px;">Conta/Grupo</td><td style="border-color: #999; padding: 6px;">Grupo de contas da estrutura, em árvore</td></tr><tr><td style="border-color: #999; padding: 6px;">Real (Ano Anterior)</td><td style="border-color: #999; padding: 6px;">Resultado do mesmo período no ano anterior</td></tr><tr><td style="border-color: #999; padding: 6px;">Orçamento</td><td style="border-color: #999; padding: 6px;">Valor orçado para o período</td></tr><tr><td style="border-color: #999; padding: 6px;">Real (Ano Atual)</td><td style="border-color: #999; padding: 6px;">Resultado efetivo do período</td></tr><tr><td style="border-color: #999; padding: 6px;">Var. x Ano Anterior (R$)</td><td style="border-color: #999; padding: 6px;">Diferença em reais contra o orçamento</td></tr><tr><td style="border-color: #999; padding: 6px;">Var. x Orç (%)</td><td style="border-color: #999; padding: 6px;">Diferença percentual contra o orçamento</td></tr></tbody></table>

Com **Exibir % RL** ligado, a tabela ganha as colunas de percentual sobre a Receita Líquida.

As linhas seguem a hierarquia da estrutura. Dê duplo clique em um grupo para expandir e ver as contas que o compõem, ou use o botão **Expandir** da barra de ferramentas para abrir todos de uma vez.

Use a barra de rolagem horizontal para alcançar as colunas à direita.

[↑ Voltar ao início](#sumario)

---

## Visão Mensal

Distribui os mesmos grupos de contas mês a mês, de janeiro a dezembro.

![Visão Mensal · 09/2026](https://ajuda.sankhya.com.br/hc/article_attachments/43502990792983)

Use esta visão para identificar sazonalidade e localizar em que mês um grupo de contas se afastou do padrão.

[↑ Voltar ao início](#sumario)

---

## Visão Por empresa

Separa os valores por empresa, com uma coluna para cada e a coluna **Total** ao final.

![Visão Por empresa · 09/2026](https://ajuda.sankhya.com.br/hc/article_attachments/43502990794647)

Use esta visão em grupos econômicos com mais de uma empresa, para comparar o desempenho entre elas dentro da mesma estrutura.

[↑ Voltar ao início](#sumario)

---

## Indicadores do demonstrativo

Abaixo da grade principal, o painel **Indicadores** apresenta as margens e os índices de desempenho calculados sobre o demonstrativo. O painel é recolhível e acompanha as colunas da visão selecionada.

![Painel de Indicadores · 09/2026](https://ajuda.sankhya.com.br/hc/article_attachments/43502949484951)

<table style="border-collapse: collapse;"><tbody><tr><td style="border-color: #999; padding: 6px;"><strong>Indicador</strong></td><td style="border-color: #999; padding: 6px;"><strong>O que mostra</strong></td></tr><tr><td style="border-color: #999; padding: 6px;">EBIT</td><td style="border-color: #999; padding: 6px;">Resultado antes de juros e impostos</td></tr><tr><td style="border-color: #999; padding: 6px;">Margem EBIT</td><td style="border-color: #999; padding: 6px;">EBIT sobre a receita líquida</td></tr><tr><td style="border-color: #999; padding: 6px;">Margem Lucro Líquido</td><td style="border-color: #999; padding: 6px;">Lucro líquido sobre a receita líquida</td></tr><tr><td style="border-color: #999; padding: 6px;">Resultado da Operação Comercial</td><td style="border-color: #999; padding: 6px;">Resultado gerado pela operação comercial</td></tr><tr><td style="border-color: #999; padding: 6px;">Margem Operacional</td><td style="border-color: #999; padding: 6px;">Resultado operacional sobre a receita líquida</td></tr><tr><td style="border-color: #999; padding: 6px;">Resultado Financeiro</td><td style="border-color: #999; padding: 6px;">Resultado das receitas e despesas financeiras</td></tr></tbody></table>

A composição do painel depende da estrutura selecionada e da configuração feita pelo administrador.

[↑ Voltar ao início](#sumario)

---

## Pontos de atenção

*   A origem é contábil: este DRE lê a movimentação contábil, não o financeiro. Um título pago aparece no Fluxo de Caixa na data da baixa e no DRE na competência do lançamento contábil correspondente — divergência entre as duas telas não é erro, são bases e regimes diferentes. Por isso, os números desta tela não são comparáveis linha a linha com os das telas de Receitas, Despesas, Fluxo de Caixa e Gestão Financeira, que leem o financeiro.
*   Duas estruturas diferentes aplicadas à mesma base produzem demonstrativos diferentes entre si — por isso, números de estruturas distintas não são comparáveis diretamente.